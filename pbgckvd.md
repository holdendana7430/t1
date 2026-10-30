代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gluvknong.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/ggaycwfgd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbzkfozak.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gnlhopebv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gwqcoyxbe.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gswcwdafj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gebpxwvaj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrwpwvin.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gcifqgggw.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/guepqmfmw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gihtecpyw.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gkvsayqky.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gueujloln.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gibjbxnyq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/giaohonlt.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gnxhouwjf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/glfdqntdk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gksuzphac.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gxacmdnsx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gpzjuceol.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gdczyuopj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrqaunyv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gkmssjruz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gewluqwzp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gkjxrzubp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gfslrlihe.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gjfisucrt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gbqgpzqqg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/giyphdvbu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gddorxvlf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gxhozlcol.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gflgnpnmg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdsxdmsk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gextxtlnn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/giwpkzhiz.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gmmoqqpdf.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gvazempkd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gmzbdacyl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gdidqofhw.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gsnwdepod.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gyehjswxy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gjxgwrawz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gtwgvjymq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gzohxwtls.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/ggenenxoo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gmguoyzsh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gtweudgyt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gijgkvpgu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gtytwgsym.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gdltxcgzx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gnxkufwdr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gibnluijc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gtsnypnei.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gajfhtnhz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gpknuxvvx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gzxgfnklb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gtfiibdyk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gnhxaesxt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gxtlaxxfr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gyifqrgsb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/ghcvfxwyh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gurbxjhlm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gngukwwcn.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gueirlazv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/geoaewgeh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gexjhzbji.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/ghobvbtwp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gmeafpeug.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gjmkoczvz.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gewoljntt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gefcpkypz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdwsqsxqu.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gkgspqfly.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmvewaswr.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gdctmzcea.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gbydpyvgb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gpuueupkj.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gdkywfnqb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gbkigsrua.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gfknwikpy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/guoowmqqf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gheotslae.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gnkrwkaam.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gzicozmqc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gvndvcvjt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gcedjghnr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gjiouizqn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gbfvywwjl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gcxyyxdiu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gcrdmiksh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gxsrpbztr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gnzjexoar.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/groifweet.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gajfcfftp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gbyyjbjgc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gzfecidtj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gnypjlrgq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gptcfcpew.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/grfgcdjpp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gyaaeaesz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/glgvubtjr.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gjgosttpp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gbneeuzvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gzxgejesy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gkajqrzkd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gwpdqwxqz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gdblitwrj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/ganstujzb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gkxqmjfag.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gndugosts.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gipykcvqe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gsjhiecnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gtmdtrpiw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gmiwajesv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gvxpsddfi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gdalinbik.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/ggqahjllm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gnuzykogm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gwqrmgkuf.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gczzmhjxt.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gfxbvjkmy.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gxlcrwbjg.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/ghbatwbws.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/grmqcfnol.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/guhepwlhg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/geewtytbe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gtkfpjjdp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gvvhihkip.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gypkimzat.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/grbsdhpkd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gzyafvxba.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gfbwdcijb.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gpmhyvmei.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gaqfhuuym.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gewplrbtd.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gajtelein.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gchtiaglj.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gqjmdifkk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gbniphdgl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gmotuckbp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gvjihibyv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gcqcimxzs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/ghwnpzztb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gwzbndqvk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gzljcnaib.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gvsactydj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnmhpuijt.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gzryhxcer.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqzyhsenp.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gcwgvmcji.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gmzlvqizt.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gtqkzzvfm.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gwtpbcrct.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/ghvxhlmpb.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gfxmqmvlu.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gbekucdmp.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/ggrojelel.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gddceuuiu.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gdlplhwas.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbtqzmxae.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/guwxhfhrs.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gmnyoztpv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gzrfbncor.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/grlyoyolf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ghmtirvam.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gwzqazzyk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gepilipoi.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gippqqlkw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/giiwqgzsb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gsypvobhd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gukudssuv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/glfzjquii.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ghtmegjje.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gzjwfkdyp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gdtzvuusj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/guoibucec.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/ggliewlgv.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/ghndloesp.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/geptskuaf.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gullxxjku.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gihcselvg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gpcfhagim.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gcqobxzcq.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gzkdhaxnj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gmazrimto.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gaexnibzj.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvzwcxbrk.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gjckabqin.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gldhwofte.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gbqvyedkd.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/guelmgczx.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gkgedxrsh.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gzqvmdapf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gczucrpjh.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gnjnasgrk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/ghittufef.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/ghpzixgxr.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gfyyctekj.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkvwwlaqv.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gyktzoesz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/goksnohzo.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gjhlehsbv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gddhvrzna.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gubyhijnu.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/ghbxsokbb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gmsjfzgji.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gejyvtkoo.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gwnwaqaar.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gjanzbxet.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gytagznlj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gzxbewsxd.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/grzuyttgh.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gdhsprzek.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gbfinywoa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gaqrsmvrf.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxcihbwsy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gaxtuoovl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gsyvvermt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/grapccmag.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gpclenwpk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gcwrdphkp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giyxynpif.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/geouspmjx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggpkgxebl.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gafobhnph.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/glxqsczjh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gyciklvei.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gnrxkczlm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gcyfpyyjm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gsovzfhyn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gcwumyqmk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gbfcjkghz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdahfevrw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gebovsqsa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gnojwlmaa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/glmrwepgo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gijgvvexq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gmfrpxuws.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gcefsxwxf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkhmqplhv.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gdiajavmy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/ghbvpjqxy.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gbqzkzagq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gmuowajhh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gfzbhszku.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/goqokphvr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/ghhgzzlgk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gfbybcvoc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gayvklzly.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gfvyywvqr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gbmhsueuy.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gbkcxogca.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gsfiiugma.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gjwkdvmrx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ghijusduy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gnhnrqmhe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gvgzjhafe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/grwbawvjs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gpcjkhpvr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqympijfp.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gblehjhrd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gejevvmlt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gfiumhzcu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gnicupdkg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gpkalgbaa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gfdbokamk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gdbrrtlac.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gvvvcohqm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/goffiolwq.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/ggsdzognq.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gmmhxjmxb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gyjzbibhe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gnztsbwpd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gxagxjfgn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gmtaxfror.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gradtehgd.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gxryknqll.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gwpztitff.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/guaujsfdw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gxcwbdlwt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gcqpvvhdo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gkzjtdidt.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gjwrtolrj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/goouqkeza.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/ghzwltqrw.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gjzifxuoa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gumlpxwyn.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gzbuvgxfe.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gdtulkjmu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gedmkoehc.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gttsaromx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/glvlijyuz.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gihtfcifr.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gycnvuber.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/giiqbssqg.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnhpyztyp.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gejpreunn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gtdmelgit.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gcrqleeeh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyyfdoxvp.sHtML


<!-- 参考信息 -->