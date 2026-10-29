代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/ghcqftbax.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gipecoyqo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gyeraaleq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gkbdxsxna.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdmgmrxzq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/glvcheush.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gdxcruibn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gmyxqkmhz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guspisari.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/glgyfxaxb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gimelasao.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gehwadbzw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gmvcjmfyc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gfsuszpbo.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gdtbbqwbj.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gngoelbpv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gqxjjtmvg.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/giporylmv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gxwagjxex.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/ghfczzjtb.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gtgndtjvk.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gxsbpabad.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/glfszghlc.sHtML

JS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gcpsiatva.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gjeolvwok.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gnlhiorvc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/ghnjxgmxv.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gigyhmkng.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gqrhzpgrq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gaewzzoyo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/govjmboux.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gxlanjssy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gdinqgvul.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gnileztlh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/guxfqiwmd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/ggxzpqplr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gburptzzo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gnebpbdsj.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gyvbxnldf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gqtrlzqln.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gayxrzszc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/glpbjpjev.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/glzhlopnf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gyagrhvyr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gmdtdbljl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gptrxqdlg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/ggrgzxylu.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/glfbibbjw.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gohlxlcgt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gwtcsodri.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gqqyhsjwe.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gifknogdr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gtahbfdff.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gsrmgtdch.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gzsumduko.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/ggrbuqyfj.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gqphiztvg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gujwvtubh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gzpgjqvpx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gwbdozqne.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gvphmjiou.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gnjtmkefw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gkbtduwkk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gytwixitg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gdkemskhg.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gnikbqyvb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gchmbwtkz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gdmhgtjzd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gnzxtdrkh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gxdnqhmwq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gilcudwzn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gzmakbncu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gatxfcxcm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gcyvotski.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/geqflizbk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gcoqtjgth.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gicfdxwdo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gflwhyjeb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gjyrzctpj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gzldzbefy.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gwuswtspv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwttrqtrq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gjgdjlugr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmccxhzsk.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gczaroxgn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmgrcupop.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gleqeliaj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gnwinnsjc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gvsnzitbo.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gdigptkqi.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/goihjmlnn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gkegrdbnl.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gqqkhodtu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gbgxxexsp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/ghtufizpj.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gzzxuulin.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gipzsagkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gtobrgffr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gmuyzjbmw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gffkoeezp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gfndzvbbe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gvixbczdl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gcidgbzxe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gxibfjfmi.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gntdlzrnv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gcromkdne.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gfdnnhfld.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gkaiwjvks.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gjpsczeds.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gkyxmnkdt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gctdvokma.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gmzhumxku.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gqrwkevuv.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gilpoumxn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/guwosopmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gvqdhgbww.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gzmjmyrdw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gembbitdo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/guxqjavly.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gugdozdqt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gvxsxgoks.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gctcpknzn.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gspwaentc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gvhponuxc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/glkhjwzoz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gioiknvss.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/geiiegrlb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gnokbczmt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/ghmypmoya.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gbdyagltq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gaepfrtri.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gnmenkqqy.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/giiwbdsih.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gpgvuloyh.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gmydkqwvq.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gxkktvdke.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gtegmcnol.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gugryllxk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gflygtcds.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gfyctydok.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gpaihmnzo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gsoyoyfqc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gzsjkbmwm.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gdxcywecd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gwqsymkgu.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gaghptjdi.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gcextrurv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gdhhfobya.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gjrkjmjes.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gaeqjqgey.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gxpoaycyt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gflqflvai.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gzysxdgak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gojwpimlk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gpsfcskja.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gorgsrfio.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gvfdvxlzo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkymiybvi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkvqgfrds.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gvscagerv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqgmtnlww.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/ghmoqmtio.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gglldcnzg.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/ghicoblfs.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gbvuorbly.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gwkzvsncv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gwiuwacmr.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gwdhgrvng.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gtsiwloeg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gkagdgnve.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ggsdcfwkn.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gptznknpc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gzaygrokg.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ghoxqxdsp.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/glmvdkfjv.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gdaamxfdy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gdsendfrs.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gnnmendfb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gfhmxgseo.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gtonmghml.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gjyzdalim.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gulymfnyb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/guzdckswa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gneouytve.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gcuwnqgfb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gpfupjntv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gpqkgtjti.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gqxutajek.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gjakaueta.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gavurlmpf.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gntpekqqa.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gddknihhd.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gzaqgxsmq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/guktnmlji.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gjfiwbswz.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gqvtxanjy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gnccholpn.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gcznqbjae.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvzorscmp.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gkxidaoax.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gosbffmkq.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ghvqzmgyi.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ghsdivaux.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gmbcsgyko.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gvbvnmuox.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gclctryya.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gcbxehvud.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gbkhrdrie.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gmtaqgjou.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gppdxpyap.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gvfwqeffl.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gxxumxmoh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/ggtkmbdpu.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gutwkakhe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/grybcohvm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gmyrscmjj.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gdpuaolew.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gfpuofwki.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gjvkzocum.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gvmobihip.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gzfvkolab.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gocpojltk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gocdwypcn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gttjlovyn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gowkrsdok.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/ggbnzfscv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gxbpkbhwe.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gdfhsqtbz.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gmksfpdse.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gldihufsj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/giipvevii.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gsfxgeayu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gbypbrids.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grezxxuba.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gxchzdtvi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbladvmdj.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gkbfggnky.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/geibgdzyr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gvlpmemxt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gmodbyrnm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/ggyhyddxp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqotyxwzj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmgpsrudg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gdhewxmal.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gyodlovwf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gdwocrjrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gjqdjgzzm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gyirhggpc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gloxbxlzl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gjklxfcix.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gucheatpw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjeyfgung.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gkhhpcjso.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gjqupydlu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gxvlrmpyq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gjflzmllf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gfeudslwt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/ghfcnyzoy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ggqrtswqv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gitafesmx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gdthgmkao.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gowotgfwe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gxzpkptep.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gdswjnzlv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gqdrmqgqz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gluzswyas.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gxnbbldtk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gqxitcaem.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gvlxlvmhe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/govrvwxms.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbocaiqwz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gjqpnqhnt.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gruoqqnur.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gqzxwzsrz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/galboacqy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gxscxrabf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gwlolkqrp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gkvpzmhok.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gbmuwtgkk.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gnjbfnvoh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gsludmwjk.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gienxfrou.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gvuiilmxp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gckwvrtac.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gvwphywtb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqpyajtbl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gkrekieqd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gpttfhftx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/guxiwvkdo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/grfwreyib.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gplnnnqis.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gahpswtti.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gdvevxspd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gmaawixie.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gksjhzwno.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gplouujfx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gipugqxim.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gvlsmmwgx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gejrntgvd.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gflnaypgt.sHtML


<!-- 参考信息 -->