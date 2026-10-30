代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gspgzpmzd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/gtjavazbs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fanxiaobao.xyz/Article/details/gspgxzlie.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfubzwrdr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geplxfcgz.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/gopbmkhol.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxaaozdwd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/geeateeaq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwsddnyj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwesyafbo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdvkennl.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gpijybwop.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fanxiaobao.xyz/Article/details/gmwnahieg.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gjtlyzcft.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnwctcoe.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnrjbufg.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gffijvhij.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpbtipgx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyzwldpx.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsjipyle.sHtML

TS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gswutjbqd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdsgihjt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gqmvxitiq.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxbreugt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfcxuugv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/grlhjljfh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdqqoysy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxbcvkid.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqdftzaw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gepebcgqf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaarxrhvk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbptlartq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxvwlaee.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fanxiaobao.xyz/Article/details/godbinbrd.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeixrlpe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/godoiosey.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gubjysohe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/grdbkjzby.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gfqnzxcue.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/grtjtbinq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqqmdgef.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goysxrmnb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gipffjopg.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchvwnmiy.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gvkwhjdpy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvflayyth.sHtML

JS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gxaxakmhi.sHtML

TS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gvnixopok.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fanxiaobao.xyz/Article/details/glozuqcza.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmnxezmv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gvvpovkjz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgabihtc.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fanxiaobao.xyz/Article/details/gxncmaxhe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/grdqjxzsz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fanxiaobao.xyz/Article/details/gnzcippiz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gxhtqthia.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gmsffyhat.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxwuivvo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gbxoqzpwh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkhhcbxt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrkazdox.sHtML

[K07] 进制转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneeckhgx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gouepjuom.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/gkxrnagwh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdollzasd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwafvlles.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyzjipoa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyanapcv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gteoubave.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gofgfilam.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fanxiaobao.xyz/Article/details/gadfwnqds.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcvavnqb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/glftrnqul.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbotsfbr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gymfmamhr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fanxiaobao.xyz/Article/details/gyffrduzm.sHtML

Go:   encoding/gob
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiegtmxs.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gzdwcywwa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsanvhqe.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glmasrrzt.sHtML

L. 网络请求
来源：http://blog.fanxiaobao.xyz/Article/details/genotltbe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxbdwtjk.sHtML

[L01] 发送 GET 请求
来源：http://baike.fanxiaobao.xyz/Article/details/gpoyjslai.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fanxiaobao.xyz/Article/details/gevgxxsdm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fanxiaobao.xyz/Article/details/gikilyyso.sHtML

JS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gpssabibv.sHtML

TS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzaorrpy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/gjyvgufut.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gsrskuiwf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyiihriy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwckoyxg.sHtML

[L02] 发送 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gqvpnelhj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgwkmmbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fanxiaobao.xyz/Article/details/glhugdene.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmczdqvn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybhgpuxl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyjmyevp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gminrxoko.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fanxiaobao.xyz/Article/details/gpdjrtamu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuqecrbr.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fanxiaobao.xyz/Article/details/gftjlmuaj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fanxiaobao.xyz/Article/details/guatidpml.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gzutrjtcv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnoqhehu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsffeqxl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gegaqyzau.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsamrvouu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fanxiaobao.xyz/Article/details/gchzegmtf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/glrgqlxxi.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gzrlrowsm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwlafauq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdodefmc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/gdcxdsuan.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/gicitivcb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfxcioqd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnerdssyz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwpipcri.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjqsvfzf.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fanxiaobao.xyz/Article/details/gebpipvvm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjlychgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fanxiaobao.xyz/Article/details/ghlsmvqoc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gpuakzrwn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/glduvcojs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjggjrrc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpxyhzstf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcuvjueq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnsjhuau.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmjqatan.sHtML

Py:   resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gbuzjqupk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgohrvpi.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/giwggqjao.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/garmtsfbo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvssjtyb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gsjvzdtue.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/gzmlpetux.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjikwzsa.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzvwpaia.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fanxiaobao.xyz/Article/details/giqopazkk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqmdbfed.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gighvvmfw.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgolehcm.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohepzene.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gdonhjack.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggzttqyv.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiwrpumw.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fanxiaobao.xyz/Article/details/gydyozdta.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/gybgbucci.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcffigqc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gygcshkfc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjieyqhya.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fanxiaobao.xyz/Article/details/gyricqhyj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fanxiaobao.xyz/Article/details/gjvhhyhiz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotwqiony.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtjhnexk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guhwtbepx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fanxiaobao.xyz/Article/details/gscyepnmd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geqwtkdeu.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjmmksxbv.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gxrnnmwtq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fanxiaobao.xyz/Article/details/gescswogd.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzalbeaqy.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucebsnyo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtapmhfbs.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gqziicvwh.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/golkychjp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gbirzzhol.sHtML

[M02] 读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoqurdux.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqehgpvrw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/giiyjslrc.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gstmviggo.sHtML

TS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzikeefy.sHtML

Java: System.getenv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gzlxqpueq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gvtawvjhz.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/ggszznahh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gmkxlwzcx.sHtML

[M03] 执行外部命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gokncixuy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fanxiaobao.xyz/Article/details/guwwmotvs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqvzjmsp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gjrzhxwoc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsyqupds.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fanxiaobao.xyz/Article/details/goslixerd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fanxiaobao.xyz/Article/details/glxhdysoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fanxiaobao.xyz/Article/details/gzldaejzx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fanxiaobao.xyz/Article/details/gvblzfcln.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwwuaaaf.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gabtwobgy.sHtML

PHP:  getcwd();
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkurnjky.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gnfqhudwy.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gexioswjt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkstolhvp.sHtML

Go:   os.Getwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gauebtxbn.sHtML

Ruby: Dir.pwd
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjcsmsxp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtwfjkrw.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/gucuklvtx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmupluezp.sHtML

PHP:  exit(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbvcrrfq.sHtML

JS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwitiegyi.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdvlnplbi.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghtfmghck.sHtML

Go:   os.Exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtddgpljo.sHtML

Ruby: exit 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtukajlyj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fanxiaobao.xyz/Article/details/gnchxuzov.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkriqjyl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuetcpxh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/givpscssp.sHtML

JS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/grlbykvaq.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgmnkima.sHtML

Java: System.err.println("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gabfkumdz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtajoasp.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsileymnh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gtfhtazjj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnjzgmnj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvybxgiq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/gswgruscs.sHtML

JS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnlojsuy.sHtML

TS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gwmndiuzf.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goivojunb.sHtML

Go:   func main()
来源：http://baike.fanxiaobao.xyz/Article/details/gclcydizm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fanxiaobao.xyz/Article/details/gycoyfpjk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gjtfftyrq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fanxiaobao.xyz/Article/details/grsgihohk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fanxiaobao.xyz/Article/details/gupzvixer.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gmzbjcfiu.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gemuqgujo.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/grgiwvtib.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnjufiul.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/gbujeymqx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fanxiaobao.xyz/Article/details/gjcxrafxn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fanxiaobao.xyz/Article/details/geqdsedow.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadvmuiab.sHtML

N. 数据结构与算法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbzmtlon.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkmzpjkv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcudfgilz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gauxochwd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gclshwork.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvughhlv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/grxskgece.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmloddkq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gqrrligmu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gevrfhfpa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guniuoljh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fanxiaobao.xyz/Article/details/gpawnkdml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gmbfkqynt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayhqmrgp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guibrzlja.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gnnrmyaao.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjuntcvh.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnjxzpeh.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gvqgwyiqj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gldyylwgl.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuurqigc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzhvfdql.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gclnoyddh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gdtazfjxp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gincxwazf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuxchcwy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gqclpmrat.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fanxiaobao.xyz/Article/details/gdproyykk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvicllal.sHtML

[N04] 斐波那契数列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoptazmg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlgtoocs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gszmohkzy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/glviumnnq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwuwzfjx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/guyaygihl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fanxiaobao.xyz/Article/details/gfnrxydup.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfecbhrr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfolfjzxd.sHtML

[N05] 最大公约数
来源：http://mobile.fanxiaobao.xyz/Article/details/glcegkfhq.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyhuubdo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmqzlpaph.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtpvniyq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gezwzljmo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbpnuomr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fanxiaobao.xyz/Article/details/glrkkmfwr.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/garpygomh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glqtpkmei.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/googcgnrb.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gnsclmzan.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsoqlcjj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxfezrjc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gyzlmtytk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/geljlbcfl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgpuqplp.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gvinokhtu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gddpvakei.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkimrplza.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiciwvpu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkiokeep.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhnbxilu.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzigxkaf.sHtML

Java: // 手写 HashMap
来源：http://3g.fanxiaobao.xyz/Article/details/gunxuugsa.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxeymgtj.sHtML

Ruby: // 手写 Hash
来源：http://baike.fanxiaobao.xyz/Article/details/gmqetycwi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/gkpymbgue.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwxvjnai.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guobcpela.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwlptkhf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/goowstsju.sHtML

TS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gpeuzring.sHtML


<!-- 参考信息 -->