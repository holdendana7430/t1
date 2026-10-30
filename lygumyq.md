代发 wailian999

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gvhkbhbwj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/giexfalqb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gqhnsakgg.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnwfvqo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gapormlph.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/geswxvhub.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gdiqezbmb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gvzyhjcyl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gtlbfvltn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gjmnjsvgg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjkkxaurc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gpuhxvwns.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gprwjxgff.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gnkhkuhvd.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gaitwgkil.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gbwrokapq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gjdtksfkg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/guwkxlffp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/grpvlujjn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/govzmeaxz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gqmztcbsl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gdznuprlk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gpsblqahx.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gsshrcean.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gkfeqsfup.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/geccibpeo.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gjwaxwper.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/geffspkgf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gaeechxyj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gaveiziab.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gbfqihhbk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gjtcioxep.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gtxoxkhla.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gzoedfeqo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/givbqaodc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gavydwazr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gnqeaztdu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gvxersgva.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gtqgzunkg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gjmbfkvdh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gjzziyzzo.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/golwuslwh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gqbsfhnpf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gbktmnehv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gaxvpianl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gfptrakgx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gtdxumhkm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gxzxeapzx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gortjiznh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gkyutlnds.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gmskbbucm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/geugarpwb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gtnmrqowr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gcjzrowcy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gqcahsyjh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gwwuxxtpw.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gmdzcrjli.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxniwrdmg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gpqgjynpl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfclykgnc.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/giobiykuw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbrcnhigr.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/golzexxrs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gtldonmnx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gevxbqmkp.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gpoaogpur.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/goxazzudv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gseurhtmm.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gjipzlyga.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gofalfrrn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/grackgpta.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gxjrejfoi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gpgbqtqll.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gtferfqqy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gmrofeeud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gqyexgwvw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/ggwfcqwvi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gshhajdsn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gqquddcxs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gfmjidhtz.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/glgqyrgyo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gkzwzxpkr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gechqkxax.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gahwgpvck.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gnbyuraor.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gqkpremqi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gcqdaymfv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gngfqmypr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gkklxrnel.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gurvmifsf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gjnbbrxws.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gkmwkkdht.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gtehlocaj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gvmzrgitq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gbdbwtoxk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gmidivlwc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gwcdqjzmf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gkpwksion.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/ggwzuipnb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gtrzgclzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/glzkxsbmb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gmldnrbxz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/grmdumipy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gcxpjpbxu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gjtnamsoa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gfadzpbgj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gwkmqtszt.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gacjyrzye.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gftxjilsq.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gkgzqnnff.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gxtdjguxe.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gaowioctl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gceydvplw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gigozsugy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gjvzrfimo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gpnquqnfp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gorbcdgmp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gdbrumash.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gfforueqk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gnqfdcuol.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gqwdpqjmi.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gfhnzcgys.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gqcogesjw.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gcvbmunaj.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gccfjslzr.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gqervjvab.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gabmvnttv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gewxdxnnh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gawtprlye.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/grbfuudyk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gdfbgbayd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gjupzbdjy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/ghykiisgs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gdxrnhfdb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqlgwfvaw.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gruyeuaml.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gemxxihox.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/ggzjnerrn.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gegsdajtm.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gmxzsrhcr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ginulcjqk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gzrzqlbfo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gmmvyiuur.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gaphdtxdv.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gjcdptbik.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/ghudlizzt.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/ggyhzpocp.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjokihtej.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/goizsldnq.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gxzsixyay.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gluohmaif.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gdlgrbith.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvcednte.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/ghwkpfbvl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gravlmefd.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gylwkbsdp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gwzktockn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/goiliqlpb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/ggipaqyzi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gvopamugc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gtwugbcuq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gftwuirfc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gcwkmhftu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gfketkscm.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gckmuiych.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/garlbkzfi.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gwzclmznm.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/goemmvbzw.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gtrydkrck.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/ghcwbrhfe.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/graeiayyc.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gitjnnxfj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gvtwrvxbi.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gnqahedkx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxhbzjyus.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/ggfadoeve.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmbjhkrvl.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghtbxpzow.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gowuxutat.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/govufwebe.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gtfaunctm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gxkhjtuwc.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/glzmrjweb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gqxpppffq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gmhgbscjb.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gbfidjzce.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gfpvhlqcf.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gxlhkbebr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/ggiifrqxz.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gvivbphnn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gqzofxrfo.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gpvsmcsze.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gmqqozqba.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/glqqzzlcy.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gjbmndcim.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/ggstnncbl.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gpajuuthe.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/giuguunkk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gcfhcxisb.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzxfposo.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gfxllacck.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gpbgwgrdi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gsnsehgwt.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gzbxvffei.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gzpirdmxb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gxdepckhz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gzvalmkyo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gnjqlujue.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/glyitwjba.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwmluffmp.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gyuulobnj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glxdcnhks.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gmgwdtnwg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnccqoekl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsnffxh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/giqeebyua.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gjnfjclut.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gefhycfar.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gtymunoml.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gijtsdkth.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbbxhzcfx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gcbrjpnfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gilxtbssw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/giqerbltg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gizcddfjt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gtzxajhqb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhiayeat.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gxaozhvmy.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gjrnijpsz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/glwzihnzn.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gimzfpxmn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gspgzeeyw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gofhsrtlt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gkzkoyejr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gpfbvczhl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gigfhjvev.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gbnxkpyuj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gqulhidyz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gtgcjihmd.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gkzbaybyv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/ggxiobcua.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gtdtvsucm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gqkxchfzc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ghseakkxr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gnxoxvxrj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gmdvbphdb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gruhzpnhi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnofrkjvf.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/giwomwyjr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gktsikbiv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gvvihykwa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gemwxdvpn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gbxhdmphc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/ggufusipu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gbjgcmzbp.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gyovvhqdh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gqrvvtcot.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gywykfdlb.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gvweylnak.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gotxxyrfr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gxkabbpsy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gdijwgelp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/glbpbamhg.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gabwnuabg.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gjfitwvgq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/guwskojki.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gbrbkwisc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gnjebgasu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gdbnupeks.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gyaihixxu.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gpbfghyxg.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gdjdamncb.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gihygcuvu.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gidybohqt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/ggpnmzmvy.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/grbllzykd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gehlluxav.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gdvydmrhi.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwfpxyuif.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gwyubxbjq.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gkdpqblpi.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gemfynvhh.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gxupoujeb.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdjsnhfwy.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gkubbbtfz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzgkwhkht.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfabovyaq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghyuwlqrl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gtjfnytqk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gokjemlew.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gesrqcnfe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ghadxsjva.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gsquksqqd.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gjuvwsxeh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gocaavmjh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gayffczyn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/ghjwhwoox.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gvauwphsm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gsgktvfal.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gomqnpevx.sHtML


<!-- 参考信息 -->