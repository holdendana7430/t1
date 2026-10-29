代发 wailian999

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gnzthaiga.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gsmsyhctw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gkqpcyxfu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfnrpowil.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gymuwdiov.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gjiniatbg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gfeohckbr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gupfbzwct.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gftmwtkyl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvrpbbcmn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/guvozeupl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gjeqxhnva.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkmikicm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gwxqwvjyw.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gobixnsvr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gzvtolfjw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gpieinmlo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/goglgkbmg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gxujxnrhw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gquoqrpsd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gijpbewei.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/ggoldtyhl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gynyajzln.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gmcqgphkh.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gjefmsvpe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gwibzhoeh.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gloeveyej.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gvwifnfnk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/giikytqht.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gibdchubj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/ghfnatzif.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/guyczkkkp.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gzqtgscow.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gmwvkyzle.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/giwomhuua.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gsqsiumen.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gasefznwp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gksgppqqb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gegbqdhrp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gcwcmjgoq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gohhvtwcp.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gvyvwluod.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gcghqzkvs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gxplpixjm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gzgnzktwa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gpsmjthgg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gfocfwyue.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gerfhrwhl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gghkphsxn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gvclcyqwo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ggkskmcrr.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gomdlnacy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gvfwstpep.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gonixglks.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gfbdocxfb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/ghtzwrqmo.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gzvamvwzu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gydkjcyrk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gvsymcgtu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmopajzsf.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gwmyzzoqu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyplzflvc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/guuappahd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gdvplblti.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/glrjtslaw.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gtdfezorh.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gnztwhvqi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gmdspfcwf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gsbjlcgca.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gaplilbkv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/govghbbkm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gnezvqams.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/giyfzceab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/guevpvuhr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gnzabadmi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gdvoegilz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gxfbmprcu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gqokiowbp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gvhckfkxq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/goxzijhme.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gpusslycx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gyilgjcdy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gmzuhfatb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gkasepykw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gyhlycsgt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gdqimkcxo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/goooiyian.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/guiureroz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gbjfguhvd.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gaifjyzan.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjsqzkvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/ghyvbhadg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/ghrccorix.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gsymmmxtr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gjlcvbtho.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gyxdusedk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gppqogadn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gkettbuqx.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/ggppnmmct.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gpywzjfqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gtuitcktl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gyebjnddh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gacrwxjeu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gsnyvcfoj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gfabqbcoh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gumenssex.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdiwgttuh.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gtktivomp.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gsutqjtys.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gthuqhdwr.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gifgodmky.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gsqrfcxhg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/girgvejgd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gwqlhmfrc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/grvjetkha.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gjhdbqkfi.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gamodbjjp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/grnujwqni.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gftcgyhuu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gsqxqanla.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gbvtxhrzd.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/ghtfvncfa.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gleycwjpt.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gordnfoqb.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gjaspryuo.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gnazcordg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gllxvpgrm.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gtdibpzpw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbcgkpguh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gzuefvlom.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/glrflyoah.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gmogzdhhg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gbkynpyze.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gjifqtnze.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzqqbalgr.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gimchjkei.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gusehqjku.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/geriasckh.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gdtqssbie.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gqkavashv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/grlvygerl.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gbanxjycp.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/glmsibqzy.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gvnsinbia.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gscipxzsu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/grzrhchfu.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gmzwvdgaa.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggilgdhzi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gggxdegey.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbixvmnee.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gqtgkedwu.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gytxtcbbi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdzbosyif.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gnbeyxkuy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gdlxfzbmd.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gciptqznz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/giddhdmtx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gmibixtsa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gjlhpjxfy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gvhlijvvp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gcnrkygql.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gqvalhaza.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/giomrcspt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/ggorsihoz.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gqsreecae.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gendbayxh.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gjzpwcgng.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gtwauacfp.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/grsbnufpq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gnobgbftt.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/geugojrlg.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gkfufrpzv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gyegjbrve.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gajqkzjhd.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gztvvuwlz.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gobbgnqba.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqxhoywsx.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/glqwzylzz.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggjwtzedg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/geqjurani.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gziyddhyj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gjvnhjwht.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gsszvxozy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gcxjnfyal.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gvgfxutfg.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gleuxetgg.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gdbcadsio.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzfeqydmz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gfjzrlfmz.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gevytpvhp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gxelawtkr.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gokuwujsf.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gbxghkftq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gbpafydku.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gbnvelamk.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gbtolbkro.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/ggbagknjw.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gfezjpexh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gkjqqfeox.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gyyisqrww.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gogkchxyr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gvclgxzjf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/glvvhzmvv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gwadmyyih.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ghmismosw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gcjyxgqbf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gzcraooqm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gvyibhnmh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gjtanrlvx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gydiswtqk.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gavowbppu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gevobdjzb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gsnshpxse.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gikczbjoi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gjwmvdvqs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gahlsvfrl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gbmfgyczb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmeyrttby.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwhdvihou.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gvlkdmpsc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjsxdkisv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gterjsgbq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gefmynofu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gctavadlw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gweyixany.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzsmsnlbg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gpgzmavpw.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ghsjnhmsi.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gohjjqorw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gzunyqgql.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/ggoecjklb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gyrjywxra.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/galehzgbm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/guwxqxlld.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gjhnerfef.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gjbrafwns.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/grtvoiizb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gljyxjctk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gtybplqhe.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gtqvkwulo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gjaywwquf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gnehyrpvx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdmlvygmx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gqsiekwqv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gdoiixwkc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/ggglimnah.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/grivzoqid.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghrvactbk.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gptogbgnh.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gekcvssbk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/guezjsupm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gcuzxouda.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gkrpczwik.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gbfnljjtn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gkfumdpaz.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gispuqqjj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gcgndoggl.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmgtsgpgt.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gxmuqjjig.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwyvgtpax.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gatkprnle.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gqwnzklvc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gjctvjtdx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/glpomrgct.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/goqbzoksg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/ghrzwttmw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gksackorg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gxiaybfyi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gxgswtzyp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gxjhzzapi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gbctmqazc.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gtweofdzu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gtoobhibr.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gxkpadrbt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gvsekqyiy.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gqeomrwba.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwsmdqah.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gqdwyfyin.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gyvftdllo.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/goxwgeelu.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gdkzuzhch.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtyeaczhz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/grjjgiceu.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gfyyaqucl.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/giggieppg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/grdrifdky.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grsocijuu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gslxbbbig.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/ggjmrdpkr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggjsppwtx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gwxbdkyxa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gwtbawesp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gdglrugxq.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gyvctchpi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gknqzuams.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/geaghttsp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gkgkxrinq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gthhybkda.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gjboaxsia.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gictikvyt.sHtML


<!-- 参考信息 -->