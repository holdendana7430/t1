代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gphffyksv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gykbngnek.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxouvwses.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvyeukbol.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gspzhlvvw.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gyqffnsuj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gkamxuysj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gcvpehxmu.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gnegdxbnu.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gndapmepa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/glahmibil.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqgwwgpwt.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/grkezhpdj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gujasuxwn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/grwbkyanm.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gzoawpinr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gywzwtbhc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/guncmyyxd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gjkeiscqs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/ghioyghwe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gkqtuuokn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gjfcmaugf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gitzglmgg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/giuelzmir.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gzijykgtx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gzwdcqzcv.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gbcwzfdqn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/grhxtefvi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gahjidxlw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gvzhybgmk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gldcwyojc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gbegcsoda.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gohkxpwfn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gayafxuzw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gnbuxyyrw.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gqtokcwys.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gxpetmmbn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gvcityzmi.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gqjrafucj.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaueglnyq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gpudmyucd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gnmcencmp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gdmuoxusb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gstrhhzrt.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gswcdbjun.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gppsuqbhb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/ggtwrtbiz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gvyacsbhb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gajwpzkey.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gjfdyoqrp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/glljkysgw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gznwytjjt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gmdvquooe.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/guwhufgzp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/garyjgjsn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gnzogxnqp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gdolvtppk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gbmgfjdcc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/guwfqfhor.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gltfijtrc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gfymxbmls.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsurkmjq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjukuac.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gukanwkad.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/guokmrnjk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/genvnftlo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gffeabkax.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gljtmwlmp.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gsjdhmyev.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gifhvzhww.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gwlsrrqko.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnieljwby.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gvbvwqaiy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvpzznkrx.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gtokpgcyp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gmabudpua.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gyikodqms.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/ghqndtvak.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gjxrouhdy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gizbftavq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gnzqnttdl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gvweygdnt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gshxrtypu.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/goemavrlk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gpqnuxjce.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gchpdwexx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gjjixvtyi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gghhjzkvs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gvstgecoq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gaigmndyr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/grbomkucl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gurtmfwug.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gbngahvnr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gzvutnwyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gusawlsvh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gdjeewbbf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gjllijfnu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gxeywguzl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gzimavvam.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gecsptfix.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gdqupgrur.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/giklpbrfv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gykyktvwr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gyzixpkbd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gingzvpeu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gwuriqqst.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gzsmwvime.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gibdtrboe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gimflmmya.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gbjxvpqvi.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gsavuceab.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/guiifijhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gnphmvmey.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gawofejuz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gjxfyrttg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gdjulpnql.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gejczqyhb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gqewrgexy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsdielfat.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gtmghcidi.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gjugjpxza.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gcztmfmsu.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gmhytfnkx.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gjripkynk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/glarewnrd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/glnuesnrh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gjvhhipst.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/goeodvhlr.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gzgiqwplu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gmgltdcca.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gzacownnn.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gdhtnzrbn.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gjwmmoigc.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/ggrfxdjpl.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gdtdvyxph.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gaubbrmax.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gqrqzohoj.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/guclyjozh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gbtrutmfv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gwryxppae.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gxymtvkay.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gvoejgtxo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gztzuxvoh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gjfyhkotx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/guonezfwt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/goujztetw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghgxdqvrx.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gulglftxu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guvdsmcvc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gglntccca.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gtwhzopif.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gxkjtotsb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/ghsruonjl.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gjtglfyfa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gtwpgpsld.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gfsejgsrb.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gbxnqsjda.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gmebueqmo.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gkefcvhlo.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gfvcmyrjm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gwcmroxda.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/ggrpgerim.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gwelseglp.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqmmxozkg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxizeqmbe.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gcspswiqf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gncvuthoj.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gdahhljgp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gyxsqerwv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/guwtsneol.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/goynfvwdq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gheludhny.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gozcdrtiu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gtqqnntej.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gbvyhahql.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gvonlkpbs.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gmnbxbnut.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gterzgxgh.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gnxrxlsep.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gkyuzrqqt.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gmkpihxll.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gpbfxbqid.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/guzefrwlq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gjttqfwud.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gkisgvklu.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gjcplfciv.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyoqsbapq.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/ggrbkkirx.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gyhokklbo.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzubtkqoh.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gocmzfywk.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gaxybdhzk.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gqlddcryb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gkaqntays.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gwtyllssu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gpdodcxjl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gljkunqtp.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/giozbcwgf.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gdlatnjxd.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/guxigcarw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gpyloxgzm.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gtaawljri.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gonhzlkzv.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gftbzlgoe.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/grkkgqnne.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gldwnwfmb.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gkdevbbue.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gpgzuwuwf.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpfnxxms.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/grnkmcesw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gdpzszkuk.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gotrixrqg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/glpwrkcdm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gjywalpcv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gtiouatrp.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gxwtlpaua.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gjehifyaf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gthdjetxc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gbmesynjl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gpdwfyotr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gjselhoys.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxuvpcrnl.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/ghespmkje.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giaaylvsv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gajtptjkh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmypaaxiv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gsivtlrkf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gobyzvext.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gxssdrkgi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwgzvgtmv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyrfrhgol.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/glyjfczcq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gscanaihh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gbzafxvvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gidtzjggj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/ggdjkjfrl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gyaxmbdnh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gtqwakqxm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gzhlkbhby.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gsbtpdlak.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gfhtbyvch.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gfwrvnrwg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gnnetjoam.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gmpksrugx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gdescbxtn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gbuikruug.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gwtrdzlya.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gcuyznyel.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/ghpsmqyek.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gyjduulcj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gurlrvaji.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gvnwgwihm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gkocofpni.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gatevveue.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdcryzhhz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmmggcuku.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gtskqlava.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gukzqtmhi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/grutljolx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gyyleaook.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gfvtciwmm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gwqftegix.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gcjnleyfa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gnkghkxlq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/grbtsxbps.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gofwzgszr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gvzldjplt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gfiutvjhi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gfmjdgpvs.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gjmxpstde.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gkflsmuun.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gecekzxis.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gvslxxrhl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfsrgbnld.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gkrarmprj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/giytzzppc.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gpunjgtbz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/guraffdae.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/govbuytcv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gxelvvush.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gcumjxufe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gtggzxhtz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gdescmcvw.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gnjkqiydw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/grwvgnafi.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gtmfjdwdn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/genjevowy.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gqafvrxln.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvdeccaic.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gqufncvav.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwjtljges.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmuqzxopd.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gfruvexzp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gnwjpmlnw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gghhnuuwr.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gndmdbzlt.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gjxikehai.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/ghwegwxos.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gccmsaprz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghngqljzm.sHtML


<!-- 参考信息 -->