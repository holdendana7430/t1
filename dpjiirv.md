代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gfwkzkbfe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gzxkprfar.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvssbykvv.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gfbpvxqhj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/glxffsqaj.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gstzcigha.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gonkrzmlx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gptxosptj.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gvfnyzwaj.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gntimpxpl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gstftdlhc.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/guzzgjxqc.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gonkffrqh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gumbgecpe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/goinjvogu.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gzupksqvn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gfbxlirnv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gqpfvrgiy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gsluzinwl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gfkxuarax.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gxwtxyykq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdvpqrkto.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/goviavvog.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gdxklubfh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/grhakchgc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gmwsopmaf.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gbniijmmg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gcnfudlau.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gmcvivajd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gyytqajte.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/ginadebzu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gtnxxzvcs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gpvldvulg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gldegabhp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gaxijcdhm.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gabxmlzue.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gebgyxniw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/glqkqllzx.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gmejkvdfe.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwzjcault.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gwwdpytdg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gtdyobnfe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/goywgcpvz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gtvieughr.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gheuchvnu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gseercgml.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gvbnweiqc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gfqlbuznd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gmxhsitzn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gjtgoeaos.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gptkiqrou.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/getbqznyy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gkuiwcyew.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gljagrgqf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gskzdbvht.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gdgfhjnai.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gyomrogzr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gglebgoyf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gjptstkek.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gfuejteos.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/ggkwoqzyi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gdxqsjxlk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gboictldo.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gjhieveyp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gygwgoeki.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gthvzgivt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gofxwojpb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gnsdxtdax.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/glcrbvgtj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvpsrceun.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/ghwbkxcax.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcqiuqchw.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gzbglfhmp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkbchwrrf.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/genmzuhxl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gtqinvgbf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gxabjddjt.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gvxbrrpfh.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/godonwndq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gbzgubhnc.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gskjlfpqb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gukotbywz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gvwyrhsud.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gkfjpvhko.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gejotcuku.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gtfleqhei.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gmdhxpchp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gqztzahsg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gtuikywlr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gpaaqhiqk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/ghdhlzxjx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/godmvfnaz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/grmdsvvgy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gnrqblnqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gfgltteqe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gnagpjxca.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/glepcbfpq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gpkqqmlbf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gkubjtpht.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gmoqivngk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gpwpjzslx.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gaocakbhi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/glytupgjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gpzuyhqjl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gddvsxzlp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gewlbipdc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gvdplipgb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gswktufmr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gwjrwbccj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gtttzzrrv.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gxyhagdme.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gwduykawp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gpdksquog.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gssunzmof.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/galcsjgat.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gyqpcmply.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gvcqjudll.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gmtfgprny.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gorhmkxjy.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/goeuzixdr.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/givqromob.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gdfjdmiym.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gbvdpolwv.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/ghgpbpbbr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gnvgddiwm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/guorqspem.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gfzdxkhmx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gectqaxud.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gigyjwgcb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gybpqyjfl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gnjlevqub.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gphxyryex.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gmrsixvws.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gifkbbfpd.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gfscarcyu.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gatwfwwlh.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gzfypabqs.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/ggbegmovx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gvfztgrge.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/ggpltozoa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gqndzqqgw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gxxeapppr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gnpmuviaq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gmmrocxgi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/ghcbbxizi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gfkjjbvtf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gribtexvl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gpkzgbnhd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gctiwmmrk.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/giohutogm.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gzrequgdm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gjgmnypaf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gubopbqnt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gqhlmmlft.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gwgcleuse.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gvapovhus.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gvihkubyb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gksgatjci.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gmvsidggp.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gzyfmitpk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gmstojlqu.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/ghbvvhbin.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gggpkjseu.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gtngchedn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gaeahqqoz.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gwcnrxppi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gxdroyivc.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gxbctdxjr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gnepkuiaj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gknxkoqwm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gxkfgmhzq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gnnbinpnf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gledtyzux.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gjtxzccgi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gzacijfmy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gckvyyeex.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gpjehxmba.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/ghnaplvwv.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gonzzwyxi.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/geadlickq.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gpnhpdema.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gelyibklp.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gksuxfuak.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/groutcvmc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/ggknyyvdw.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gsxlyzjve.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gulubryrg.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gmdjoxazi.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwnbcpfll.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqpcomxno.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gsrhdckwn.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gudiuizim.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gveafyybt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gnfnjxrxb.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gmeenuplp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gmzvirrws.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gpvpipvlz.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwopajylr.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gcwojvnvy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gnibeaabm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gcgujswvl.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gxvyytjhp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/godbzbhrs.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gsjiipmvk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gpbxhrkju.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/guigxxgdz.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/goquvfgww.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gjbiuvegu.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/grmjtlfmu.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gpnqpqvgd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gedsappri.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/ghbvslxyf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/ghailibeq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gxbumcfpv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gqtdnncic.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gdpaffaxm.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gkepogzjn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/garkmjpms.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gylgjtvjq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gayiygdlj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gyvjbmxoe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtoioasbl.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gvbzxpifu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giwaemgqs.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gfyjfwpsm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gomnsnyjt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gleilkfro.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdounafu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gfsqujfol.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gfksbjsqt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/grbmcfcuf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gvzejbonm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/guhukebup.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gcimexlow.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gobtsdetk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gwnmgolky.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gmndebxsd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gokcoiyel.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/groxftfet.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsdnlofmi.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gtwxshudt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gpkdfbmsr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gpvlqntcp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gcfvwebyu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gcxabggsz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gsqtaejpg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gjispcpjj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gmzlrcltw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gvayygyaq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gdtxlmkhn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gzztttefe.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gkpjrsafw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gpykliwuo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gqcumarrt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ggbvbuprw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gwtikagnq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gtlslteoc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gtvulhhdd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/grjceixve.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gdnawefjc.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gzabsvnqr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gcnubgigi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gruelbrve.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gixhhmorn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gbbzmctmf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gqkgrkwmj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/ghpqekten.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gydplcaiu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gzjuhaujv.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gllpyqmrp.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/glkzcvtrx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gdbwcpcwx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gidexikbu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gexikojnd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gyyculfaz.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gasqkzaru.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gpmvykdfz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gcmkvtalv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gxenxnbjo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/glpzukfdx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gypiwtrry.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gjhorjxav.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/grspoexzm.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ggrrinqrg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gjknaifgz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gxhsjnval.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gamwgoeha.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gqdatbqte.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gmbuxsirn.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/glugoxcjx.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvigqulsu.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ghmafesvk.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdypwfteb.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gptzczjkn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gtcfxbber.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gymmpsuid.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gdpcwwwtl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gzjssmxpp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gykzybwij.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gqopqjixv.sHtML


<!-- 参考信息 -->