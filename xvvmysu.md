代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fanxiaobao.xyz/Article/details/gikjotzvt.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqnnoavn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/gggnfdomm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gesjjzobq.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvgzvtbw.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/goxadlanf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgmkvftl.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvywfbxjr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdswlvhqs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblcywlsl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/ggwzicfgu.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gslgpgupn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdbsyfrq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gaejkatyg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvsitcte.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpmzhrpy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gflgoslbq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxhyszqmc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvkgfrdd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjrsaxvd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvpuplcp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdefrgek.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvztgqhr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gwiddmljz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxzvdczj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fanxiaobao.xyz/Article/details/gjapileda.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/geoovuccv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzeqerxy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjscmbaih.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gaqbtawnm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fanxiaobao.xyz/Article/details/grvetxtev.sHtML

[K05] 深拷贝对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsidbkhg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvhzpaii.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflijfras.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/geylvtzby.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuviyngk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcdfpyyc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbdnjsha.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqhweqgh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fanxiaobao.xyz/Article/details/guwxqniqu.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fanxiaobao.xyz/Article/details/gvsiuiags.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/glcaomjpw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fanxiaobao.xyz/Article/details/gahnrhgfd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrwgkyf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/grgytenky.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fanxiaobao.xyz/Article/details/gipyrvtcj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/guhnblapj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gthjfbglq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcsklyrh.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmsqdvfuw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gqnpwdejs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fanxiaobao.xyz/Article/details/gdqrjxxcl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkellsfp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgkwpbls.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gckrtxond.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekblwbcv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gpjilpnnn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gtjvvfjjo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fanxiaobao.xyz/Article/details/guczikycl.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsyuohlc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyzzgqpd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmxvvwok.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwulszjv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggghoyquy.sHtML

Go:   encoding/gob
来源：http://www.share.fanxiaobao.xyz/Article/details/ghswpjaja.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gawtkowhj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gpijnwnua.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaloddur.sHtML

L. 网络请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gorghvnfg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glgkjdmmz.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmguzeuas.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwtrbjfh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fanxiaobao.xyz/Article/details/gfycdbyst.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdgglldg.sHtML

TS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnpackxq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fanxiaobao.xyz/Article/details/gzagnzftg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyvdhkhr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fanxiaobao.xyz/Article/details/grooftofr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gmexzgxpo.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gfhicfxqf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhwoluwz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fanxiaobao.xyz/Article/details/gatqnvacf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhrzqdfe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gkesphmrd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsyritwt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fanxiaobao.xyz/Article/details/gnlwhxwmf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzieljsxa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/geemttbdb.sHtML

[L03] 设置自定义请求头
来源：http://blog.fanxiaobao.xyz/Article/details/gfaoxexed.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdknszvlv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gqqgewkzd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gilmxizer.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylqzywlp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fanxiaobao.xyz/Article/details/gaahqqsvb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gnneuzwvq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fanxiaobao.xyz/Article/details/gppnjflzq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gybjlgzyd.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiubydpz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fanxiaobao.xyz/Article/details/gjiefyywq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbynomtc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpkivprf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gnwbgmdzm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gxdjrizgd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxtiggpo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpxughaj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmdkyutq.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzqfylxm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqdghrxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhcfqxuc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/govaeitcu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gylmhbjot.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiisxere.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsypbrqhb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsotrhauq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gdcvwwlqb.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gjrabslvz.sHtML

Py:   resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gxskgxibw.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/glzpaqzzh.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsikddvt.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gdcixfcgd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfxtiado.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/gmgbbfgqj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fanxiaobao.xyz/Article/details/gvwpssssw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxmnnlah.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gareurdoe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fanxiaobao.xyz/Article/details/gyjlidgts.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhwdbpdo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxkkvtij.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuyvkdum.sHtML

Java: resp.statusCode()
来源：http://blog.fanxiaobao.xyz/Article/details/grccziqhb.sHtML

Go:   resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/glwwatoau.sHtML

Ruby: resp.code.to_i
来源：http://blog.fanxiaobao.xyz/Article/details/gsqhkfhqj.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fanxiaobao.xyz/Article/details/gjppysvrv.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/gjefifnbo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/gncrtwmng.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fanxiaobao.xyz/Article/details/gcabyhgbn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gjhyekkue.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsqwkxis.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fanxiaobao.xyz/Article/details/gggebihss.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gxzclwaax.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gespljecm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsrbqgdr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcgwmule.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmnunuid.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gctnloxxg.sHtML

[M01] 读取命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkugtclbt.sHtML

Py:   sys.argv[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gxetktlwt.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fanxiaobao.xyz/Article/details/gixzvzcjw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnlnghri.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnokyqxin.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqybidcfi.sHtML

Go:   os.Args[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gnvymihek.sHtML

Ruby: ARGV
来源：http://blog.fanxiaobao.xyz/Article/details/gtroirqyf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gvvlrsogs.sHtML

[M02] 读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghdtadwzu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqenmtjud.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/grfuixvdp.sHtML

JS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhxcoknf.sHtML

TS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgowwnft.sHtML

Java: System.getenv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/ghecioquo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsgvumbi.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fanxiaobao.xyz/Article/details/gunttwnjh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/givgenkmu.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiccntkw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnpfljro.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gykijeakm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbemftklc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwolxlowv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gblhydstq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvxipcxn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvjdtzyg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcptaued.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gajmtidpn.sHtML

Py:   os.getcwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gouxvfbhy.sHtML

PHP:  getcwd();
来源：http://3g.fanxiaobao.xyz/Article/details/gljoordlo.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkgkuocq.sHtML

TS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwggucmy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gbmdrqhqb.sHtML

Go:   os.Getwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gfdsdcsac.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaatyvbxj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fanxiaobao.xyz/Article/details/gmhzxubwg.sHtML

[M05] 设置退出码
来源：http://3g.fanxiaobao.xyz/Article/details/ggcjfguks.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlthqwiw.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzokeebf.sHtML

JS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhewzvqt.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geedzxrfh.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghlfqqjpa.sHtML

Go:   os.Exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkntqqvrn.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glarkmksj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fanxiaobao.xyz/Article/details/gahthydmp.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqexfejs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gciifquwq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gntdwaszm.sHtML

JS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gnlgtoapp.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbwhjxlj.sHtML

Java: System.err.println("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gucsghxdp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqyqydhm.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/gwmsiypsc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxwuixnl.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fanxiaobao.xyz/Article/details/gflbhslde.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fanxiaobao.xyz/Article/details/gglsfxgmp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gqwptmqus.sHtML

JS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyfcoxzm.sHtML

TS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/grwvultyw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gncbhyncg.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfleifqnz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/ghbbbdvjx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbcatimk.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fanxiaobao.xyz/Article/details/grmihfnlz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvuodlbq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fanxiaobao.xyz/Article/details/gplzufbrv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gevwcwpbz.sHtML

TS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gxvhqskrg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdozzuicq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gvgfdvmtc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfmgqcbj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fanxiaobao.xyz/Article/details/gzruiyfmj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqkpbxvqw.sHtML

N. 数据结构与算法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grieianoc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcpjwykse.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwclvhjb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/geiitjsvg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwljhzybp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gllcleiuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnukitst.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gqihepvuu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grgyhpmuo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/gicxjwmei.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyyxerhw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoapyvee.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgebtrpa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdrvbkre.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gwgcjbhkj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzuyyzfu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryvasnkq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixznmerj.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gmpdehger.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goznqyuxu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqynuazat.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeowplgz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gxscanczl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gwwaijjug.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gjhxhpdyt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/grstltuuc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmjbmyzq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fanxiaobao.xyz/Article/details/gktxdwtct.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsejwqzo.sHtML

[N04] 斐波那契数列
来源：http://wap.fanxiaobao.xyz/Article/details/gqyecqjta.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuwjzmuz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfrpsjhf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gwydootlb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gkscvzchi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcvqfcvr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcpjtbis.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslfxjyjt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gdmrqibil.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwtbncqm.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfqdrtbv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrhzecaa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gppbmwrhz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcdtdesib.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtizkivg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfmwnnvw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjswfszzt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuogllpc.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfodywblh.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgvppokn.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqyzqheg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/ggqnczskv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeiqlnsa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrxaycvv.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fanxiaobao.xyz/Article/details/geognvbik.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotpriool.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkiebvpg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvodpvlum.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhkolrcv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiwvwwjg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyhdqlno.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fanxiaobao.xyz/Article/details/gahqktypb.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsbqwcrr.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fanxiaobao.xyz/Article/details/ggidhwwwd.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduujepxi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/gfbfuggzr.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/gtpdaysfo.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gvyldhzdd.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskkxohof.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzmxbabw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gumeyrhlo.sHtML

Java: // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gzpvsorqs.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuzcctom.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzpeeqxc.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gweffbglc.sHtML

[N09] 栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmrvgcvx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcgwqmav.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/giixhhybk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gpzwwrjfc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhkufcyk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gffmfdhmu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gfivkcjso.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gcosexnfo.sHtML


<!-- 参考信息 -->