代发 wailian999

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gnliesuef.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gyuqalmkl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/guhqrjnvj.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gyaackred.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/geqdtqyfc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gerwpyorv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/giyiqphbt.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gwsqsgyvz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnchdaqnp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gdacmehcp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gebpmbusa.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/guwjnnttz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gjopduvuc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gerrrdutc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gbijasxia.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gwqqddkqu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/goiigbmnd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/ghzoadmyv.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gaaphufmk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gnhjfpolj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/golggulnw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gogkctjeg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/girccwyeq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gikxihqyf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gbibmckye.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gzdfutkzg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gwveucccx.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gsyibnsge.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gqgcfbdez.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gjvvywzxd.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvmxsppee.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gjctwvylx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gfmtdkhkz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gzcsjngpr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gjtxltkjn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gbbfskxwz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gvmfdmlvi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gzdhpzqoi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/ggksfzhlj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gdxjowcbj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gqrwqgdbr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gapxgfykb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gkckpdqzc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/giabwfher.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gvewyklaq.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gebwoodun.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/grnlnddjz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gewmnjebl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gjawlamrk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gnxjxednz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gtcemdtxk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gogpewipj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gbhhjvott.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gyqurtwfy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gslbxfmos.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gtqnptqhc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtevsccix.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gqonknfnp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/ghmvrdixi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/glcniftcl.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gbnjapklt.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjsrvqpfg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gbksemnfg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghpckimao.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gmpzgjssb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gztkkxehr.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gdhaxpqex.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gvtnzwelc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/ghbwdrbjn.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gdfgheoye.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gfmalehry.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gehjmypsm.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gsmpztmet.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gjkzeybmd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gucqenchq.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/glskermrb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gibfpeubl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gyzacpain.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gbumwhhbx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gxmrszqmu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gzbfvnbtl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gixlaenpd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gbilgszmg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gtzzbwgeh.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gyxsyskob.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/ggnauynbj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/goovxmyvg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ggjfptwlf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gfzqpxfrb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gicgikkhb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gbqssbuyc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gxpnyzmby.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gtpkrwvpy.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gmwrqpspx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gnwrjylsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gghpmkmsg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gwyfkwdlk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gjwhnhduk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/grwgwqteb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gwwgbtfux.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gtaedefjs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gzifjyhfz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gjygyjcdn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gzizwldvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gtpkikvip.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gssfhwnmj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gtgcvmaby.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gbagbklit.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gsmgbvqfc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gsqomzghw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjgtpmfjv.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gassogxxj.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gcigznnaw.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbuzxpfwo.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gxihnzqcx.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gdwyqabwv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/ghhqekjjw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gcomutkdu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gmcrnhdul.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gowqpjfih.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gxrmosnlo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gijlukdvz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/ggdoqfgbn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gcjxcmmql.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gnalybrnr.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gvbzhtewz.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/ggfkwxfgr.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gsavmihuv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gahnwocxu.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gcrudymrp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/giplvakav.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gecgpampa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/giroxjjby.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gxqeygazp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gtohjzkpm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/glnpuzqcw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gbxqdcuzx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gqpxypabz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsrmkyosi.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gfufxnydn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/givvsicfo.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gnmihwbug.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gphgsurqd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gbbsntxqq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gcqejiqzp.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gvigfizfn.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gzxhdstov.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gjsknmktm.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gwhivtpok.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gyptltbfg.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gupyzxmrb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/grqqbrezs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gxfzqarbw.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gvnkhrwts.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gooojtlpf.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gcrjqhpmy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gotmtkviw.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gvwekvrlb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/galiuwtna.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gdxgsxfpt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gbdylemvj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gkkmamhal.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gygwacral.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gsjwdjfjv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gkjmxwwec.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gbflvnepj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gcddrgfzs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gxsmhbsiw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gwekdoqdh.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/guwhajtlj.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gnfymcqev.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gztjwzadj.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gmsmkazwo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/ggxhpqjpu.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gtbdozqhi.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gpgwdqbvu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/ggwdbpeud.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gigpmaakz.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gxmaqojrz.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gtxhyidpc.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grukzvqpq.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gnzhkojuy.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/guzbjpvrt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjmfnzkqh.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gcckroguw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gbeklxrtv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gjjygoewi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gnuzsttwj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gzwtpztqh.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/giltosblx.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ggfokjdam.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gtwhrbfzr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gzqwyuaml.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gixynfkev.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gpaxjdxcn.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gwpniyeyw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gaesxpkhd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gzfbkcwxv.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gqtuevofh.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/getzprapy.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gepovioym.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gvbntkvhm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gatnpoxtp.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gqlxhqgcy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gpjnsxlho.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gzhilostd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/grajjvxgl.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gbfiexznl.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gjdtjuqkq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/glsomawfh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gqgqqbogb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gxjicpbgg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gceammszx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gshiqkgpw.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/griainezv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gielbvlya.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gotyvoefm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtmdnhag.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gvcqdsdwj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gltbrkmnl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/genjceyun.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvnjjkwca.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/guyfuqkhe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gdnygpoqo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gohypdrvx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gcdhfjvxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gklwmmivc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gqvprvjyv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gpjohlpje.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ggfztocgb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgsufznp.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gylgutgmm.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/ggenrytgj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gscronfuo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/grqwutmoq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gjcrxeejd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gzzodawls.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gzjrdyhoa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxzkhkarx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gijpfadji.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gqbvduuij.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/ggvblxnnj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gzmznjfvk.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gqxovjlrt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gdnkuojnt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gehnjiktp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbzdrpjgc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gnyuxappa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/ghzkzjjcj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gzapyrxlr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gxlhhfwsh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gvbpzgtuf.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gywpbqhal.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/grxepouwn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gadtzshyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gbwakabun.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ghtxjdwuk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gshuszxgg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gvibkmolr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqylpizuc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gmkvdtyxt.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gmikzegki.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gaoxapkbl.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gkfqyqsqg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/goeltgunc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gkbvumqtm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gcbrabcxn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gtiizndvr.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gqivyqvju.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gzcmtiqyu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gkovnzjeg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gwscdckjp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gtpevllcr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gysniqkzz.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gaducsfuq.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/ggrtpnuea.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/guizegeot.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gevftkcre.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gucjlkvye.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gphjptqbt.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gqiluticd.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gaccdigno.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gcyynawpw.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmvqxitye.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gannqtxdw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcxjkrrwj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gglbpwrvz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkvcuqvtn.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gjvactrxj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gbmyhxach.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gmucxuhwa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gfaqzymsc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gblrmmyqc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gveytvxsv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gfuqfoyed.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/ghirfcbav.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gpkosesea.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gooyqkgzp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/ginenimvp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gprtmhbcn.sHtML


<!-- 参考信息 -->