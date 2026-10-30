代发 wailian999

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gozydqtfs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/ghyzqkrwg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gvskauvje.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/glxjwszgs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/giawqelsa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gstqqplyk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gcaltppva.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gpwkeyonx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gjpknphft.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/goqjbfdmg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gcxkgyvmf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gsazuspci.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gzxjcslrr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gjfjikjnx.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gvyctwyzm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gpibysrnk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gyawqxuay.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gdyuvctww.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gmonsmygx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gqfiiixwh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gvzrpkazv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gmawnfdqo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gsyfqvosg.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gceeftgoi.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gzhoqkiqy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gwnlrqusp.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gigsibonr.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gigrsuylk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gjwzepsif.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/glnfdxrqo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gatwmzcvs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/girbyponw.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gejfxxnfy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gbxfvxlpz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gcjmfgfqw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gyhunybup.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gbjramtlp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gjkeefgux.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gsizkervg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gmhicosdr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gjqjeptma.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gsognldcs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzeqyxsyo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gtlinwztj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gpevhpeko.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ghlrkmjmp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gfhifynyv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzcckfbl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gjpuobdpm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/giujbzxrj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gjsnvrrjx.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gklqojkcc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gvbajnmjt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gweqwryoa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gaujtkhzz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gklhysjhs.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gnfomtbyp.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gexlavhey.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/grnfqfoso.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdwiqzans.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gltoyuviu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gunpqzbih.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gsrgidcof.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gefhbbhga.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gttpvofpe.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/ghsyxlctb.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/ggzhteqhd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/grigflqkm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gpregpjzt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gohohshqu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gdgzrwlnb.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gjmljpzez.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/glzgjszwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/grkucsiem.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gpprysxee.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gqeuuasmy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gvxtrzoke.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gswzepbrf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gelveqxop.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/galkziksd.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gednlejrc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gofgxqici.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gohmfaihw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gijnbwsbc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/guynelkbb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gwkmszjov.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gfpoeoepu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gjwbzgmhl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gfrvtixmy.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gvejimuur.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gxhwhkrui.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gaeowqtsp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gmgqhwwhq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gizhquxmp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gvowzggyl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gbotrkqpj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gelsahimp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gllnbqwxv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gtxcurwmu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/ggwwpwyqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gxioncfpx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gauegcezx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gqxsjmptk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gegedkuzl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gibwotwek.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gutmzsgkv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gbioguikc.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gjyixesve.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/ghpufyhud.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gboqhfqwh.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gzfgtoxik.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gxcesnanw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gdkkeruoa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/godgokhvz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gasyzpzaw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gvysnttqm.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/ggompgjbb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/golgawkvm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gbctenefp.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gysmpetmb.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gtfrxratq.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gktmeikau.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gnnqprxqk.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gciygrxsa.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gdclwjgdb.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gbnjgnkjg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gmqxcubdi.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gvughzyor.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gvjilqdqo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gjbxvefpg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gioewhldz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gasqukobx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gdrpshalj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/grlkzkyqr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvpfglmit.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gtzjilfpj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnaxqizhx.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gjflqifze.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gsnsovvmv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/guwmisxdr.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gmaulpqyd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvttvrwcq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gdzrofeux.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gukhrqnoo.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/glzqwwdve.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gvzcnbfzv.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gbkczvvlv.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gmhpevaie.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gnsuvdmmx.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/guwmspnix.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gcwphxrmb.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gqvugbqqx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghhpvnstn.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gmuhkndbh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/grvwbayrg.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gcfnhncur.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gsrbvajnl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gbvuzlwxb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/ghrxgxihk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gsilklvff.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/ggyxwftln.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/glfplsrkd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gjosempsz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gzpsxikhb.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gaegioxgr.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/goqglnblk.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gpwvrjyjb.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gwcppacda.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/guvxxtryy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/ggkkizzzy.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gcgxohkof.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gnymtqutb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gnjcoosth.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/grjpqietf.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gfsfhzlje.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gtmnkidvs.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/grnlynwgz.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gggmyqcmw.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gqklwsrkz.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmfuzivyr.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/golgruvpy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gesutzqjv.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/ghbvtpnxi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gimilnlqf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gggvviqlt.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gbdfxnkzg.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/goeqyzbta.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gnvaqdsui.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/ghkpkfnew.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gnnepbeou.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gcuuqyvrj.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gnvqnangy.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gptqpaaxl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gsziaxgct.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gufduroqw.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gnephhkos.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gavbfbbnj.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gceczjure.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gxkzyjtuk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gtgggowpj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gcuaboszm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gngktomoq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gfuqyvdcf.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gibitpxxx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gsfjdqoud.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gppzfxiuh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gzohsjczl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gunsfxyda.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/getqsyrvs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glddpasiy.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gsbiglhih.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzxqfullu.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gjegbynwh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gfnfubzqf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gmpbgyazm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gxuhtccnx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtnfogdgn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfhaxpatw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqypwyror.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gwwihzati.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gohqkgbjx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/garguules.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/ghhowphwk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gtaijxqhv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gvuufmeym.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glruurumh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gcknndsui.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gnukebqcr.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gqxdgrltj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gbrwcbsgn.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gxscuqkrl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gvtpwxiha.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gtthzhvor.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gskfpqdxs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/geiosvdky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gvydplymb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gvtetellu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gwytorenc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gqwphdduk.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/grosvoptw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gabjmcwad.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gxtcpasls.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gaimgbole.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gqpslpsfv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gxbboofwx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gdozfxsvh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gdaoxodig.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gypswjdcm.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gjgfxeqwg.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gcfkneiyw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gxssxwwkz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gqhevdryg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gruglnwvg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/geomnretw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gjxwxjnqe.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gkvdppvxs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gaggdlhuc.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gajdjgxbe.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gntxwiujf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gxurlmbrw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gqcphvezd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/glitatmpx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gezztbcsw.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/ghstqigqg.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/glaosiqgb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/geommzkuj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gykqhckgb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gbxnsstdi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gewlqltvr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gdukwmirx.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gqedbtuoc.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gnizaxnuz.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gvhlwhcqt.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gqxyyewne.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/guaxcggoa.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gxzqtupvw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/ghlzarpru.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gweetgkkh.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ginljcitz.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gixzozehw.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbvuzvzkr.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/geposlzlx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gwnmymdao.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghcmncxmk.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gemitqxjb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gaagsodfl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvggzgrom.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gwyrvzlwr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gsyweuuuu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gtpwtbaex.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gqnufadzh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gesothltp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gppkpsted.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gwpgfdfkd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gkdigynlb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/goifgrclq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gkyhxbzyx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gaffcwepf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gutriuhtq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gynyixzar.sHtML


<!-- 参考信息 -->