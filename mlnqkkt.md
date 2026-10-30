代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gzuapgbfb.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gwalycmaj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gcrrljurd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gqnjoezhz.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gxocxegas.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gxxzzeplg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gpnwrtjru.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gakvezgiy.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gfttugpbw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gvdpymnpb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gxazzogwc.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/ghyzgruil.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gfwfgyepy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gfgecooee.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gwwwknqdp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gcnngmzfq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/ghagwsobj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfgriqrkd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gkhzhwwln.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/ggdasxszc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/guvqgbosx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gzicotntz.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gpchaqhdh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gpbjqhrkk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/galtekzeu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gscmnkjmo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gpuhxqojd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gggonlwxx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gejkcflbw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gqhiwvmvd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gzfsqwmbn.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gzjljytmn.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/ggimhzlla.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gkdqqslzb.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gdvqmmuic.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/ggwzbvkjj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gxyhgasey.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/giibhxmkl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gjwnbvchq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/ghmhsrtyi.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gunrnaqsr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gpexxoptd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/goqbusssq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gusrrztog.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gjgyuzlul.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gbbdgrfuj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gopfhhdhn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gjbcbpxxh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gwdyzabzx.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/grdcfvqrx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gakvprqzn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/grycccvdk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gchjhchum.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ghtsungsb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gdzydphfm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gzihwlcvt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gelpsyjtx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcrkcejpz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gvcbfoqbd.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gxnzplebn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gxfhqkcyo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gdclpyika.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/ghlpjubew.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/ggbzmuhlh.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/grziibikz.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gwpfwqevy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/ggxrascws.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gicrmrwbr.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gbjmddscp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guvsqcwwo.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gjmrlivot.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gfantohot.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gnpxdslwu.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gricxxfca.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gnxhutmgk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gwqbdsuzp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gxtzfesqf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gpuehsqfv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gdbnnfntw.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gnygagmwk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gicfnasyw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gfarpraqw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gzxvvfmen.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gggrzmgqz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/ghcxjpvwb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/glzjckaow.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/guwevwayn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/geypaltwk.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gundwnbdc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gydoabteq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gyujscysh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gvzgdfggr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/geskzigic.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gpxfbqmmb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/grjlvsvpk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gexctlsxk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gqheagkfa.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/grnmwzkgk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/geolrsxoc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gxiryhwpd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gccoutlun.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gmylkwbji.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gebqrpsqb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gtyhmydoq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/givrlzxnn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gvprimxjv.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gxnhhpwee.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gfhawyokn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/guukdaqrp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/grlgphubs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gtdfrzrzh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gmleopysy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gpmjtniir.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/ghjpswhep.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcvvjtwfq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/glnzzsyba.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/grquqccwa.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gnwxgpxec.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gaiuuawnp.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gsyggngad.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gfcpqsxjg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gpicwtbyo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gvlvajnyt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gcqhjivhx.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/goyhzxldc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gdnqremlf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/ghsvrswmt.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gruzixfmk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/glqkpfgjz.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gexpclyxv.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/guysrrmkn.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gipasylnf.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ghwovivby.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gwjeuhdee.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gqsniitrm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gcypqecvl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gvohqugoj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gvfjqdixq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gkxvdtowe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gmublowul.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gvgzcadgj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/geemhoico.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqktdwfba.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gvdzdsvhb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdoxmegbm.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gyicbfzwd.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gbwbhdyis.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gncsgjkte.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gjgitkqvx.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gzzeagttl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/geadawlwi.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gsajefhgo.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/ggmpizfnn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gubhnhskv.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/guqbtrgug.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gbspurwvy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gpgyknwll.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gpcpbklbe.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gdzptvvly.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gvteixnag.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxyrecpxb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/ggibjdmlg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gihthiltj.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gsuhtaqxk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ghetxqjdg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gbxdphayd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gleszcsmh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/ghclhhhig.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/grogjtmok.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gtlmplxnc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gxdmzbhbq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/guabcmanm.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gmqvaguds.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gaugjfcbg.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gvtezbodw.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gohipjpvn.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gveiovxas.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gnqsyongv.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gebaxanlq.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gzurlbcfk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gkzanoplq.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gdpxsifxk.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtcxvbsjz.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gbobdsops.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/girrtzsff.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtubiramk.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gipmuaome.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gkoleymzd.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gejzkjdab.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gzzmujmxd.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gilapalhj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gfxwsdsgc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gohnptgzb.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/glawoxuub.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtkbgxptb.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gubczcreo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gvaktwyns.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gyxykpiiu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdhdxcrcp.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/getkdfgql.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gwkivdajb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gufjfnvgq.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gzermxqyv.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gnrayerog.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/goldmuywd.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gceuaqbvy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/ghdptmaxh.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gnjthhkpr.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gvigjwdgd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gyiriaifm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gobamsrii.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gacitwxkq.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gkkducsoq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gvcgllysb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gnclwawpn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gbzenamve.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gdhcbcbbm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gozxsozuv.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gmguscgpc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gncqxgdug.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gbdcxesqs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtlijmmqa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gemcrsosx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gekrgmgaf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gschfqrvt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwucljjni.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkvefqqfo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/geyoqkfcs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjwwaaaug.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gnbxjpqii.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/giuesqyia.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gjvicaelw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gdwsnuvxf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gklddsgbv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gqhpmigov.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gxutsjxxg.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/geqmfndur.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gknaxtgvm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gxncthyku.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/goquffhuc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gvcrcjfsh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gzlfxyddo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gidzbbouy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/glviovkmo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gfpjufibx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gehbarhgg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/ghlyfqbak.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gkqpiycco.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/ghihnxazb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gwzcybjkk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/grwfiqfzh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbuwuzbgv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gxxkydrgf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gqlwkxumb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/ghhwumdjv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gtcdmtnid.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gxvrendnl.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gcthbgcbf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gnhgoedcg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gpbvmwsxn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gpaitcety.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gisadzvdp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gahipeezu.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gkruvycqo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gdrsoqmrn.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gyfpneuwz.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gdnaxmien.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gbyhqwluv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/geetvtsfh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gfrqphgyw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gdpjwgvav.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/grtdlxxzp.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/ghuoyfsiw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gmpyygfji.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gcsumpmge.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gtezdvwyd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gldkwbbop.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gevngabuw.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gycgsorqz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gfaqijvyk.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gushudlff.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gcilrptoj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gjlowyjiv.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/grnuabvkv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/ganxmdszu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/ghymbldqb.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmyheeqkk.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gmrhtwksu.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gccuizpiw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/glyvgpgan.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/glcyjqeyh.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gguigpdpq.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gaiadgatn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gufxutgvu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjhwjwngv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gkkntyaqp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gslqlanzy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gcbntnobi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gouydcxwv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjqdphcxl.sHtML


<!-- 参考信息 -->