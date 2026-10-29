代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gpgrfdemc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gyqwpcbab.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gtdpdtsjy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gnryxxiwn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gcqirnfha.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gtjatukcd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gbqnbqmdl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gjtqrclfj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbyokcqi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/guuhxhten.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gyvqremgj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gceoizkpn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gpxktizzw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gojtfljuk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/ghpfuohmo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gkeqzfycf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gmtdrjjxo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gmbvkaxfh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/giifgzzhz.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/glpuqrlym.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gncbzclzy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gygdgxuwg.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gsvskegut.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/giwrwkdgq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gjyowptmh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gytzzjofb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/giecoulzs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gygzpwuhc.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gugbqguqu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gceyxnjro.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gqiqzvggw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gkddkarvd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gfijbzzta.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gypzguxtz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/glavismcp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gnlpjncyc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gsrcsmrpr.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/grbussknz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gvylxqncg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gizdzslso.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gxucjqgnb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/grtahvuuy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gfwdhcyow.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gyjrejogg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gkyxwckce.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gamzekarw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gvmizqxhm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqqhtjnlw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gmlnwnemz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gwgukqexj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/giurcsxth.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gayauwlyy.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/grnwkmrfl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gooxxnohu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/ggqyoeynw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjqxrpbmi.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gkebvmzfh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmclpxyce.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/glsyeayqx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gyjwwulnj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gqdnlpiea.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gpdnpqeuz.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gohamqsik.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gxawcmzio.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gqxlwvwef.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gaorvoduu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gtvulxbli.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ghbfybnam.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gdvdubwfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gbcphlwfc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gqzqxxtwg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gxtcxknxn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/giacbnaat.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gfhobdqoc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gizbbfwxg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/getiluzcr.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gxxjraokl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gpsupxups.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gxyysdfro.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gczkvgsqb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gyqwacybx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/ggkrjghiy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gtwrawsry.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gyiibbzwa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gkwciwsll.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gntrggowp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gscelgwtx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gbggfspkp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/ggpvqmnim.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gvjitofti.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/godomsbbn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gkofxjrad.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gqanseiht.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gkuruzjja.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gonnbsncr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/grontkiju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gyifpdndu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gbtvpbaxd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gzukeocvp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gqmuinzho.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gjhvxqwzb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/giyjiinip.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjsdsjlmc.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gkpcyfamx.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gdkzigtyh.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gfnmgmjxz.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gyyyghgwx.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gdtfiadev.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/grnbqaquj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gxqtwyseq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gblggxrsh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/geacrgcvj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gcerlnkrd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gzgwrnujk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/ggldhvpbg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/geononnir.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gqxedcqia.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/ghryklicx.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/goqtugpna.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gfeembzug.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/geaxehanq.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/guvvmicbt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/glzbcmjoo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gbzqxchtq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gjrbzdqrz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/goxtjklug.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gcauwfpde.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gjzkgkaaw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gnefvzoev.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gjnruxfjw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gutqvdpgk.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/guvcukjbe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gybgajoru.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/ghhsmiptw.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjofthbdp.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gzaitzfrp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gjbflbsef.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gcyhzhyvf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gbcccxwya.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gouivfdzq.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/guepcwgtn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gdfypvnlg.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/ggugxqphe.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gpgtstqcb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gmwdpfbhb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gmastteal.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gomndgqig.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gxczzkmpa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gozecdjml.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gxmzhrfvd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gehoesdsf.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/grpachkrc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/guibqtaib.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gwreenuth.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnqtddonf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gnsyccfxx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gcfvqujil.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gbrrzyouh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gcfafdstd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gosvnsdta.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gwaqmztku.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gtvzdnijp.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gfnrphjcg.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gvippuzzn.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gyqewdtbp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gbtusunmp.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gzzmcqrhv.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gabmnptnl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gwgvutoud.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gjgdfgkfs.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/grcgfiaek.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gedmsarvb.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjmhapzss.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gdatuljde.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gtkcnrihn.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gymmvxdip.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gxpvdmfyy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gfbxxevhc.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/guhcocoii.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuovuewq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gpbuctuab.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gpqajzwwp.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gressugua.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gmwfyykzm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gcsirgzbb.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gnyuoqbvh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gqogjvdzm.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gofxwaxwq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/ghqvlbvlc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gutetecfh.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/goqmwdtdw.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gsmmozhks.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gteygvwbx.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gqphfnpvw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gddrotweo.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gyghtgkim.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/glyjymspp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gufcfauzu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/ggatyfirj.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gfmhenlml.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gddmquzph.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gywztadbz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gdjafxshd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gqqfjbynq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gppowqkog.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqyxkiaxw.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gxvmzjtgo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxytsdfrb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/glebmyufg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdtnmeoym.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/ghebdegjm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/griyhlgup.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gekkjthjy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvdxjskil.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpkiquowg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/grlgdtzaw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpbcwuioq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/guvtzgylx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gkohbhsjl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gevohhihs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gfxxyirsn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gimsdtdxh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gtmsvfkzf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gyrnvadng.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ggmxetxwi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gaqtmvbrl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gzbkxeucx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gclvtrnwv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/ggygtffwm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gblikmthy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gmyfnqguz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gktdnhxsm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/grmnjiugc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gvlmbohtt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/grypmzdpx.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gzcwldncw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjlvbpkzi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gbgklkduj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbmoyqgml.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gyvwmvyki.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gtyepvkdq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gkjzgrcue.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gaawgunik.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/giifblhaf.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gviisxikt.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gtnnfikkd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gmgapdnqa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gndwghxwd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gtlunkteq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gxutegzmz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gesrcusoq.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gprghuyar.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gypoxapel.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/ggsllllki.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gvwnpbdap.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gjtkztqfw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gawmxzcil.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghcuheczl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/ggnbibsju.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gsbdnrluq.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gitlarjek.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gqdtcoqqg.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gfjpjhwfa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gguriohuo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gtwujlebz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gwlbcvfle.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/grzoktwgm.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/godrqicvw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gdxifnlfq.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gtisnkxgt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gwbfnshxg.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gkznhepme.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gxllwcinb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gurbdhptj.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gbavdbelu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzbmmlkjn.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwqyglsug.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gdgbzepss.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gvrinngqd.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpfgeycfh.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gijsfljju.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/ghvgkchxg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gqmakkpry.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gprbxhhdv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gtfxlhexf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gxxygehed.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gwxkybbfg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/grvwinncc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gnyrxijwo.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gxhjnqzse.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gsvxenmvg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gpriwxnng.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gidpgdksx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gjpzbjnyv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gmblsdthq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gitwynsrh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gacmzxgdt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gqboafwfq.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gimopzwvt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gnmgmqfho.sHtML


<!-- 参考信息 -->