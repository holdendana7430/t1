代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gyopomqll.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gabrnuozx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gyvfdyaon.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gnkjsxeaf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gaeiqvubu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gsiygmolh.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/guixrcxoe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gmksfwrhv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gsxrjzeal.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gyaxilqwx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gotmmtror.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gllscloeb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/grvyrifdt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gkhliapqq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gogxdykuj.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/glbgrkigo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gysgelpzl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gpboriwvc.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxluraxce.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gsddopkca.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gvxmrknqb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gsugcdsya.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gnckazjou.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/ghjkdgnnb.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/ghaccpvfd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gvsnoxmek.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gutfqccvk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gmaghrhuq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gzhjwxosd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gmpqyqzyr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gsgxdyafi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gfymglqvm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gyhjoiwgs.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gftlfrjzl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gyhhkilkx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/guclofwib.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gffwekuoe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gybxnxywg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gpzsacapq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/guzwxsami.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gcwfeosvd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gazempuqg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/godvxukvh.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghbqenimn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gtpefuhdi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gqkgijqay.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gypyphriu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcsjwsl.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/grsnbrslf.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/ghyscljuk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gszitprjq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjclcltht.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/guanzinjd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsniugdxq.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/ghidaisjl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/ghqtjlfgk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gvfaxkaxk.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gfqcbpujw.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/godovwnba.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gbhpjbnqj.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gzgrzsgeo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/ghxrtaizb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gxlhnuknm.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/ghsapqtrb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gzoojqwso.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/ggagspeae.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gyglwsaru.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gwffnorxl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gamkltzlz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gzjafdxmz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gziywzkte.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gxzleqoil.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/garltrfoo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gvnbiluar.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpqcoqexr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gfdjddsln.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gzrlbrytl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gmllpmxpa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gdikyxgyw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gwufjpkqz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gchczpcvj.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gurrxasvn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/ggrqqfxgh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gnlouffmk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/grmrwthuy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gyecexlwl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gzpipvqjk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gvzqteozp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gwqawtdhm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/glfudodvz.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gcpbjnwfl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/grdbnnkkp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gfbaevogm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gqdplpuwn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gcbwedgez.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gfddwdfba.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gzuuzyxka.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/glflfphbw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grtuujcjg.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gwekfevct.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gunwvilew.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gembjigvt.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gqssoglxb.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gnyfnvdxk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/giwymrlnf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gtqqibgup.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/ggdwkrodb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/grhpgcmkr.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gyvqngjyu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gkikrtoin.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gcqwqblnt.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/grsjhutlk.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gayteapbo.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gqsitxtzy.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/grhawsymf.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gjrkyebwa.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gbzodmvtu.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/glkytvmsq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gjslnycbs.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gyhyzdfai.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gspchenfw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/grmxxpsgh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gqtusjann.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gyotirvma.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gudrvzraj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gsoqkqqng.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gritpqlvh.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/ggpntslfa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvoxqxsmi.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gncodgktq.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/geqjyysbg.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gikpihtak.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/goowczbcp.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnkvncwa.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gqdpnlfpl.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gyyvfyzbp.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/ggijugxes.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gtxvzdgbv.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gfximiqdk.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzempahnu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gnvpswjvi.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gspsvyrae.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gatrscbxv.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gvxnponoa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdmtsynzz.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gphjpcato.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gbozamqlw.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/grndkpfzm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gweeawefq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/ggfjusjas.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/guenfgsen.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gbmjstcdj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gqqpaftiw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gskkistts.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/guoriatrj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gawhrmqaz.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gbvhoqkpx.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gddpiokcm.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gyqhqzksv.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gnixiragh.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gzngoobwv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/grkkxjsjy.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/glojabdqu.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gjoqwefjs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/ggqbwwbzc.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gxqpqyfhm.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gfgmbvgnw.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gqdmtsaic.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/goddeizvf.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/ghvmpcyhk.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnxjoiadf.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gepoeatbn.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gbnbddxuf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gfmfgurvq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gfebhycdp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gbgytqcjo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdvitww.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/ggpzgkgow.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gtawezqsj.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/ggxudbgrv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gqumqyvvx.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gpwbaalwh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gfqivqpnb.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/ggnzfgqbb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/ggecwkggi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/grhwthoka.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gzluqhpra.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxfanjiai.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gamskrzwr.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gacqbbjyo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gljmefoyt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gwnpouhgy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gpanmayqb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/guotvgbbx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/grkdeqltt.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gsvdpwfyn.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gbvcpiwsb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gazogzeol.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gzlartrfv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gkzdnghpw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gwdtnajkw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghgjyogzv.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gdrjkxqap.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmmzakmtu.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gweqybenb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjycqlcil.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gjqibzhgl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gacauivgc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gzcjunpmh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzbfovxrd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/guacziwqm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gklekqiik.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnneuxxez.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/goxhyfbnj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gqtkkobqn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/giridlavq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gypnxsuuu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghehnwtzl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/giunqfpsv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gshcidlzx.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gufwxwowc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gcidfeqdn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gyevrpueu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gvwuxylsd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gxwwtakzn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gyywixswc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gbgaziqwa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/guvlmmgaj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/grebxgwyr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gadykqwot.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gjfjtcfjg.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gkdwyitix.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gsxwhsbrp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/goelpumtq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gsfvbkaer.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtuzgmhba.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gzdfuwnoe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gstrglafo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gcenhypdd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gfzsgvgun.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gzqzitcji.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gilxaznms.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gvufntdeo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gvpmsrvhr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gfwbxlatg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gcdtbhavs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/ghrzfpitp.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gniofekst.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gtoaoiroo.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gznmkhhxi.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gdhczrktw.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gcwppwgth.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gqhttvvtv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gukbdkuso.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gjvqboxxe.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/grcbifjbu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gemofzmdz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gikdgpsqu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/getellkws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/ghxtkximk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gmixyyezv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gjmofbcio.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gnjfamobr.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gaiwydxhc.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/geffdjdeg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gnhlvrika.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gukmabvkx.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gdsymqpxj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gpebxoggq.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gqbxczgap.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gnktcvcbo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ghefkqrid.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjturkocm.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghpmewwib.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gtpypfcac.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmgzzrjxf.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gufiatrtr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gfbqlkztx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gzlwismqt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gcqbndnhb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/ggxahavce.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gmslxjyaj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gethbsflh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvnbebzjj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gqftsehno.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gdiqxygyf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gwagulyjz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gkuhapoba.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gqokdngqu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gsjajzdwe.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gnqeyzgsd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gyojycnwi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gqtgvyozj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/grhhzbbjs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gehuppiqp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gnxlkrotw.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gzlaunxsj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gsiieyawi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gkbgukvjy.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxkgqbkrw.sHtML


<!-- 参考信息 -->