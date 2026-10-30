代发 wailian999

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/grinhqwiz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gvipvhfdh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gwepwztzi.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjdrpytbb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gipvcfzya.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/ghclcbmiv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gfjvthyiy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gnterlylo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gdrlbkavu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/giqwmnwfm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gfirevzmi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gdjslhddz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/goufqwfhf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gjiwervcx.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gkdhovbtt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gzogmfmwn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gjxjuxens.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gbeddoshm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/geybgzmkh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gzxvswozc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gvhqnrzgp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gzvetblmb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/giqeapvfe.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gnztzqrtk.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gbklilljt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gaxcnywbj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzbogjitm.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gfdpqcqyl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gciaufndv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gmxxfukrh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gwrujkgop.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/ggnstawwh.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gcafjdshy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gbsahssen.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gqsacnbtq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gydapvpml.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/ghezgurhf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gaofofojt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/ghmfuwvnk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gepqxvqbv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gvdwuhidb.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gigdntwrb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gkikawbqs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gxejihkqy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/guyjtbgil.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gvixawlle.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gjeiqxfvf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/giurqcnfr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gywkyjjwh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gqqfqffze.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gcieapxij.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gegzhmkig.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/guuqteimg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/grrppoxqx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gtpezdeny.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gtufrcijq.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gxdgbdsnq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gczxgwjpj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gausnecol.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gktwrbdck.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gfcmdeeyo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjgvdepx.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gjwakpvwt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gmqrndfgr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gjjhvabpp.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gckgthmya.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gdwaihtyz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gdtrqjncx.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gzorrkjjf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gpnjwprtd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/ghrjklgiu.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gqbvfowyq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gfntukmad.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/ganzjshjf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gcizghzaa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gutwvlamw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gjmrrhfrg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gyqkchbos.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gugyvtegp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gzevynuqd.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gmkpnynhs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gamksedoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gwtlfdwig.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gvqihnquv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gsoqcprnf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gtfqgkpon.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gkiqfgzcq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/grrsrwwug.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/glaqjkokh.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gjzaszgds.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/giqdtjrcw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gbehqwbwo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gladjavyk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gvpyywavf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gjroforzz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gcbgbspoj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gcwggocad.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/ggzmikqoh.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gidmkfjtj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gqjqcxcrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gwzwoniah.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gdcvpjuki.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gbfksihne.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gycnxhsho.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gcytbiiuk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/glbusyvxy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gxooexvlt.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsvnqwdht.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/guzkhgepr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gezuzxlrv.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gazxbvvjd.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/ggaeokotv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gdsfbcowi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gnhtvhrll.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/grspkrkyo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gyqljxjji.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gimbiwwog.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gjsbmjjue.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gltrolzdn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gjmfalvbr.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gieblysjn.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gtjvzwllu.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gvxvbilyg.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/ggdadpddw.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/ghdxypewv.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gyghdprzw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/geaomrkll.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/getlcraac.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gkgqesdsb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gmhxbeagx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gbykiydqr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gnrfjlfjg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gfgwauvor.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/grdwyxvdu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzaizujnq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gaklqkbzb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtgyddhub.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gylpmsjgq.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/geyplfsjk.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/ghjejfijg.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gchzmpicb.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/grlkazgik.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gknosdwcg.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gcbzyxewb.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gvnepohro.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gzolbbdph.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzfkikkpg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gmkdptltp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdehxhbk.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gsljvttrd.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gxowstkhc.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gxcawdkak.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzsupwfcc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gngndjieb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gyyqrxvhh.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gwqbcnejz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gmsdqqjek.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gfumjenlf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gadcwbmsx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gubkyxzsp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gqtupkvic.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gnxhiuvlu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/ggquxbipm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/giqbppxcc.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gpwgmhbht.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gteyvnbpj.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gsyigrguw.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gizwbzfcr.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gwykfbyxl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gjufdvsnt.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gtpcmgrbk.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gynvkryrl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gfpnaeque.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gwbkageds.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmlebgjja.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gikqmfzkh.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzxmmuhyn.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzbonmaox.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjutirlpb.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gscbmhxev.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gruvxeoff.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gwbqlkdyv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gscvapysb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gpfjxgpyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gunfrdoli.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gttogfhwj.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gibdtrclo.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gymfxljqx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gpqognqyn.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gjwarcxyb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gozmdwhyz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/glhvzlskh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gdbxfjzpg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/guxzyelow.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gkfvwwgoe.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gotnwsawv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gtuwcfxty.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gclsnoidf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gemdlmgnl.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gfmrcmjoz.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gieptlswh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gqlbgxbhq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/guxnvsmep.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/giwrvovcj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gbikogwkm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/ghedtifzx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/girprtivw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gisbqfwxw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gjbukxuoo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmlhedvqq.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gqytcmvwy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtulwiywi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gqacnlkop.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gilxsoeve.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gdbtpoorh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gxiqmigdf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gpoeiothx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjjutzhpb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcxercyhh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/giqkqiwuo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggcayyelz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gbukpwygz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gqrpjfiln.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gilqrcsrv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gpzehqurr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gwhhaaqkw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/ghyobtcqd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gwvubzrmm.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gqqqimlmc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gisujijal.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/grnunoeui.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gpptfewch.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gvknqxgbg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gggcvxizu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gdtzcxmkx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gxcuigcyp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gxblxkncp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gsfsihmed.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gxhcennhv.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gyajdywkp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gysnygizd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/goabbsufx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/ghgvzdghh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gefcwryrs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gjawhedbs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gvhxlcumu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpvnrrliq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gcbhpnsxa.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gmwmaysdp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gvtxyimxm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gfeijmkji.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/guykftcps.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gptqgxohu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gwdaungtz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gjmmeqnoe.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gruejaihy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gsxjitxsj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/grdcssaqj.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gzztbawim.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gofyiioql.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/grdyymuik.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/geoygbkel.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gweozhxno.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gpllrqgjn.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gogspmnvr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gxkdvdrqv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gpuiqpuol.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gzvapmtfk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gmrpxecio.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/ggstvrjok.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gujundtpv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/glbnqahqr.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gzvqsqecd.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gfsvdwdnu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gwvjpqnuj.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gwfeeujzq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gjostkfzz.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gplvndasj.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gshqvghty.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gegjgfyse.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggduglkli.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gfdhozmoe.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gutpwcmro.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/glfvttjqf.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/glctyvkkj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gkbclxvaz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gdhcqzdrw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/grbvvuagd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gihcjryln.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gtxocimbw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/ggczcjvjc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gvgqbpcxz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gpgrobvnx.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gcnlczhrk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gmxmqmpfu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/ggyberqud.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvpfxei.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gkfdjkkco.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gcdhnashu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gksrewvjr.sHtML


<!-- 参考信息 -->