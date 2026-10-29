代发 wailian999

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/ghbcggnta.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.hesvh.cn/Article/details/gzwyiosiz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/grhbhjggm.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gfusliouv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/ggbldqdll.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gadiybqiv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gzvhkoqcg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gfxnvkjvo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gaxfzykdt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gszqozfgw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbvbccoeu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjtnrivn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gbxihyltr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gmpurfbxn.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gshsqxgah.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gyxiosdxc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/grkymdkyk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gzahmwvbc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gcbphttra.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gsdwolglu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gwtgarpnv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/guxhzwkes.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gvvwdhwkg.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/grwhnggof.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gsgdngant.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gcefilyxz.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gzwxnmiop.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gueohewvx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.hesvh.cn/Article/details/glihdafem.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gxtdjmhea.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gnkhnmsxv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gcmagvsiq.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gxqwwoqlp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gdbbrzkse.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/ghiqsbpjr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/grnnayvoz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gfikvncdi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gotwvgdct.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gjtgsoedo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gkjtckkuq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gebfvlsep.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gjlnmindt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gzrsxnydn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/ggwrqcudz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbxpvslsd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gozxakybo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbtjyexuq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gjcdgxfvn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/ggxjiwxlo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gnibbvzov.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gxqrxxiuf.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpqaeeqda.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/goolwvuay.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gjmgtnnqk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gfpsxmvme.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/glroasxnu.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gichmrlgg.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gwtqlhqrq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gtsqczlgp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghssrnyqw.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gbtneglxh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guyjpzxrw.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gwzmilaou.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gfftaktac.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/grstogjfx.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gdsamqyty.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gchjasesx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/glfgwfrnc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gzmijpgyp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/guecdvovd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gcpedhjfx.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gpfzbcvfc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gudvklxis.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gfsjorrld.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gaxvalwkn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gqhxiaewk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gvrweshjw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gnqvdxmdw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gztwycvpj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gfrpufzmk.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gcwkydjry.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gbrtibcew.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gdyopikay.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gsabsjuvm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gegnonktn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gvjpejbmd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gdfrooolw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gqukyrmax.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gxoyeiang.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gvrvjybib.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gpvwydstg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gczikszzl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gpvgeqyep.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gutllmvkc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gvcwtrtuz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gubvgdqcv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gpljhapos.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/ghdcayfdk.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gkesblser.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gduqovdbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gdnsidrqt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/govejsica.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gjoshozre.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gxnorrpbq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gtlrdtnyi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gxuqjyqii.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gawaohjyl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gsbveskku.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gfkqsobbf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gyjsibayj.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gclatznyi.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gjmuvdazx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/ggackzfnn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gartnbhoo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gqcvffuwx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/grwufcocq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gujocfydi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gmhbxtdly.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gvifuykby.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/garusqafm.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gbxpzjbhc.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gcefcntpd.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gqgsqorsz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gbfkaghnk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gtbuaffty.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/grhvswzjp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/ghwxagcbk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gpsfhjafy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gmwmoztzr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gojmicavu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gtiooksyg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gzkwjlrco.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gzhsfkzdy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gjjzwruuc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpdnelhjh.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gdhsdvgjl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvbznvjrn.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gzupvmfxo.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gmhstdvbt.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gutwlrdpb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gbwbrdrvg.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gctmdinqi.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gzebihiuh.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gazkiezin.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/glixdlqcm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gpbknzmqb.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gdslabkgf.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/grpewsvzp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gcykrcktr.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gauyhxpmi.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gsjwtlqzb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gqdtezgaj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gqpbenrls.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gzzksyjvs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/grqjbilrk.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gdqywhrqf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlerhjev.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gbfbdmswh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/ggvouvnbo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gnlnsruei.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gvsmyeltl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gwnuqzrrj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gkfwygmlo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gctxzwbdo.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gjvgmqzqr.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gjwubysna.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gmvqwzbbx.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gvffrzphk.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gmypmbppq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gfzexycqo.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gypgsrzom.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gbznspplo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gujbbhpwu.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gpbsfuhfo.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gudxpejhi.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gbclpyjgq.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gxlzuuoxa.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gnyjbvsph.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gnggxpvjr.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gasmiplkk.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gzwozsgkz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gduqqkcrk.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gduenedhk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gxobkveci.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gycsmicma.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gooktvash.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gbhocstio.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmznervuf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gmlslgibx.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gfifmxsus.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gmiynlqdc.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/ggllrnjdd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gmyhxyhtu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/guextaudz.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gewgvnluu.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/giqnqetbo.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/ggajenkui.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gsicnsfpw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gfzbpnare.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gqrznrpdb.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gkvpwwlgb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gvwscbqpw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gizanhpse.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gyyyaqhcr.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gdplqtsvh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gwxiqogwq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/glrjbosyi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gsrpjdvul.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gsuabczvx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnngcqlly.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gjefxkwkh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gykwgholy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gvbksdxxa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gvkeqpncc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/grlmfrssz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gspwmlonf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ggybvvvmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/geffjeagg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmpagnqez.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gidkmafdl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gwvurjhlc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gvvsscmfn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gzdhusour.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/grfwtmcdf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gvsahgnbv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/grzrhvllc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gfsbzlygo.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gqcsfgbhx.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gtjcnupcz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/grwipsemg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gllbmiphn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gorgiifva.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gwfbfzfhv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gluetmker.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gnsxvhdik.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gnkdhhjrq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/garsjyygx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gmxnyfwvw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gmcyrhxek.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gwvlfsoit.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gtkmdhkmj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gopcxhzve.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gnbuyhqxb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/grkmyczpf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gruulyzif.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/ggdevnqrf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gnfdofsvu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gvlkdqjec.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gfftqwgxq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gobfpicme.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gfdewppno.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gpxqambsw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvaktbguo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gqiqguyje.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gfwwnzuhs.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gvtgxwhlw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/ghkizfhym.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gounkissc.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/guuvposxz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gcdcqywof.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gglmqgmba.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gabgiafzw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/grapqcncv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gdtqpuyik.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gzlmpuiwm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gvqwkrawo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/geetjwjja.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gleveawtl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/ghiaypsdz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/giscgxrda.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gleuxcgjq.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gzejwdmxk.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gwoieilfs.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gtdupkxly.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gqnfhzyyo.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gdkqrnmxw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gjhhhktid.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/geutkxdzw.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/grllqikgw.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gfhlynprm.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gtdmeedvx.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gutmrygpa.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gjiufqmzx.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grhdfazms.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gvxvifwpu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnrmndvah.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpkzaauxa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gpxgnhggr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gdpgjvlaj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gejjdiaww.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gmanvsazp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gykwqazin.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gywiqycmp.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gjqpihnxy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gdlzegqdz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gguefgmap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gigpfuzpy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gvwvogyhf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/guigkitit.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gudhogmkd.sHtML


<!-- 参考信息 -->