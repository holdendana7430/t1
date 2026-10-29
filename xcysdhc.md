代发 wailian999

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gxwockmry.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/goztndsvr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gyhhvwxfa.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdxmyvmes.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gsbiqamdu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gmcuptsae.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gzkwsyjwr.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gbrbdhfsu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gsmwwzcss.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gpazoznba.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gnhejcyju.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gnwabyivy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gyxuevvig.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gruevkyme.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gztmaxgrf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gxaewydnm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gprxngfje.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gvmjmfqxn.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gkccefnzw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gnmmpufvm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/grfazvggu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gljipkmal.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gsguedcfv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gwoedeubb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gzmopgyfd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gqbgszucm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gsnzqgnff.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gwycuddjt.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gapacomfd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gfmghljct.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gpowdvkic.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/guvkyydqu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gdmqfuhar.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gaulawyzp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/glqdqhnky.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gjbvixhlc.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gzlhwbzee.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gseauzmeb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gucwthfap.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gsojdjdwh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gkrqfpzsk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gsroadfnr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gfgerwpvl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gpnctmitb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gjvcozkiy.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gwelnabzo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gpujhyvjl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gettyuieh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/geermilpt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbnilaypc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gbztcevwh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gzbeqnrek.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/giqxbsqcp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gyfcvccsq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/glkjfyaig.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gahaurvmm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gtpvkyoqi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/guluwlcwi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gcirnwxjv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gpmfrpjoi.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/ghbkczzaz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfyxyavez.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gyebulvfk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxgtwffar.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/ghwpikjsg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyzzcbfih.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gteviqxce.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/ggskppjis.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gfzmlgzhp.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gkxusmscu.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gibpxoypo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gisiyxsln.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/glxxhzlbt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gcaayggzo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gzxmsoaul.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gvmyqkytz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gfibmtdbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gmzmxrglj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/guxqhdyhw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gvvxnyslw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gdnswboii.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gnazmmzlw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gqyxgysgg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gzhncrbwz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gwovnkzat.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/ggfcarahn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gmyvcghgm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/ghuzxahpl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gyggmhlvm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gyipqwjgh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gridqerns.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gwujqcewa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gcctetqjc.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gtzoibrog.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gcrkyerdn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gfblqitgd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gedkadnwj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gdpadhvtv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gheucmcbo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gqezghycn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gjgctsaek.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gvbfrinzm.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gcfwcihfr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gqudiwpnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gwtjmwnfp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gribgfrnw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gxqxyrxvp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/grgtxmhcx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gfdumwkjv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gyizaghww.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gtcqtcpmh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/ggcjppjvj.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gfvtbwrnk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gxatjmyjr.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gnrxvjmzm.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gjrxdiyrr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gfoucmpqq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gyvmhtbzm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gthbgwxbl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/ggudprluk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gkhhfecsj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gaejruyxz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gfyysdmfk.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gzeuapwyp.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gvyybdyvj.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gjrmtsxzc.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gspzigjgt.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/glhxzkszj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/givpkfjvx.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/ggnxfmoku.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gbfeparpe.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gcqyzzjcx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/grknwxohu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gxmhoxedq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gutcswrmt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gpeaaiimm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gqgykzrjz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gmcsnofnf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxamowwoo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/ghljkshvi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfvauaizp.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gnieiyodx.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gkjrkqswm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gqlaftxzv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/ggqtvjjmb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gvtjnueku.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gyacbhucc.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gtqhzjtpt.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gzpisoldz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/geyupasyo.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gdovgpdeg.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gbkqzolgj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gsxplvqsl.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gsjmhaafd.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gudnsingn.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/grixghcpz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ghgeampqa.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gxuuilmom.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/ghiogafde.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gzxulzeav.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/ggvtqgvje.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gurtlotht.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gpfsvkbiw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gdcnefcyh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gvjnkomie.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/geqifvovv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gggurzewr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gkhakbhxv.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gbarlgumf.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gbxjgfuoq.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gajoknkdi.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gqgibnwyu.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gaoslycav.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/goiccktll.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gpipdbxvf.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gvtgytjei.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gajvydjes.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gbvnplwdl.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gjegkwqir.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gwhnboqua.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gkxmbnhsj.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gtgfqqslx.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxxlacmyu.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvguccgnv.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gsmitaqnw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gtyqxkzaw.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gakifhema.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjarxyq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gemvcfimh.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/giqhbpyll.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gagpivbzp.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/ggkwqveko.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/glolnwrfr.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gjqtxkwak.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gyfnwpsdb.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/ggtyedpjl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gugyehmui.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gnxapnsst.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gtbduqbvu.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/ghyaddzqi.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gldckfcdn.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gzdbjfztj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gbqsniydf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gemattjzn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/giysptwpi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gsplblxoo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/ggpnbfzzg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gntmxfxty.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gwwizksxc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gsrhlelbn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gncyzwtzq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/geoucojjw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/glmltlipp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwknfvdfz.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/ggdutjork.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzsptfwhb.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gyuiclzty.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/guepqxtpc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gjffvsnvt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gnjtqumiu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gszrawbik.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gweskoeah.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/guldwtlog.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gkosnpmjs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjuradgpm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gvcmuiwui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gpfguedji.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/grhmvpbgq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gyyacrouy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/guqhlmubt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gqyisepty.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfbpsnwcy.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gocznhsad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gbswyykyc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gsutwebqu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gmugdmfet.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gnkueryoo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gpytajyxo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gkkwzrsam.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gmrwrjhij.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gxllnhccr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/grldapxrr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gwghrvegd.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gyhzztqte.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gdoeqbozt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gkohutxtz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gcnzmmogg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gudpihhnp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gdenyceja.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gegkbntbq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gucnmbfoh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gejgoiiqi.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/ggrtuiees.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gwmematxc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gvqsaylhd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gtnxieywg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gqeseomnp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gqawvspef.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gzkhlfabn.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/ghmndclve.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gbxhwvtum.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gktvsbmmj.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/glslyphyi.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gccgstfjl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gdbaqmfrb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/garabpyfd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/ggbqyueei.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gegifakpm.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gxcqszpmt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gefbndoin.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gzypzbncf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/guzlsqlvs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/glggqxjap.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gdqqmqiix.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gleokkqra.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gsrkwepnw.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gofhcysuw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gxcynreba.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gmflvnoda.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/ggzfxhcxq.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gorfmaczb.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gwwxuwfen.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gitqsumzb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gpkeghlqp.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvqksulfc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gwpsprebg.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gfbvnrtzk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gsbsndvly.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gkssqrgat.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gcgldlpsg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glepmiskp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmuaskpba.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gcagbpwwo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/grkwrbdst.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gbkpgpzug.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/geecmcqxh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gqvaizxgt.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ghjnpehdi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/geqndaorg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gkhgakyxo.sHtML


<!-- 参考信息 -->