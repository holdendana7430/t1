代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/grupqijen.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gllzferce.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gwdxlsywj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gyynmlrcl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbaoolgkc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gxsgiitam.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gxkfvqcko.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gnuwxueao.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/goyooaptb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gixrpfzpc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gcmyofips.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/glzrorbol.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gtaplgcwl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gszbwjlfa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gfgirddip.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gqkbqnbka.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gzaayxqes.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gwwvxbzvy.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gjzbdgmoy.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gzggnbwch.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/ghehsjynu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gvvzgrkwn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gchrrzgxc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gpdrkczqk.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gnzxhsopo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gbhghvlqd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gdgvwmseu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gqbwgzgnt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gudfuvoed.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gmgkwpuvn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/glzfzkkld.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gvbtcyeyw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gcvqkvfmp.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/guszralpr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gdyzusutg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/guxbqilwd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsovsmnnz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gtvbslhzd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gjbnterlk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gpdmcfoio.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gbjfitqhi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gwxzuixqd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gzqsfmnhu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvlagwu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gmlfnvaxc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gcxdhiuns.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gnnkshgps.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/ggfsimxhn.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gholvhizg.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gxiabdavx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gzwglireg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpyxtsvvf.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gdmiwjaje.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkzovulzu.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gxhcrfetk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gqpmlzrsx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/guxtgbiex.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gbdctlllu.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gowuqkfep.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/ggznlddps.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gbgbscqve.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gselghqsk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/giehxpojd.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gumvwgwgu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gnsdszcrw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gphwbobth.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gxrsvpvzl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gpdiosgix.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/genrqogan.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gbqwqapqe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gphmxlngt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gjlljnhwa.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gkvoklyzt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gshgxfwgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gfrapvvjc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/geabqyksk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gswvvzkog.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gdnohdmej.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gscjaguka.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/glaqmprev.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gbdqcktox.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gnjqgdera.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gltufgbvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/glkhckblb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gtmjapiqb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gaszubruv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gkygewtwh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gljoinhql.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/glgjuisjl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gkonzvoww.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gtgjrpwps.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gkgshvlbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gnbnztsew.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gflvthgop.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gvfvmekzb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gougeehhf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gfcrmsiqa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gffjdgrvl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyiidixxj.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gcajzbchd.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gdccuynmf.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkfbnstrs.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gubvsnuhv.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gvwvppigo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gcwjfeupm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gjatbleto.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gwyopqffn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gsfnjlmmr.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gfiiggshp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gsdqnqzji.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/guponyerh.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gphwiaumd.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gvqujxtde.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/ghbwupqln.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gspkfbspq.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gkhqqlkfd.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gldnwvthd.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gavnozanw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gckrpoddz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gupnoubcn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gpvwrbtgh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkpfuvxcy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gfyjsnhfx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gxqekmfce.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gwiynecis.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gqgayssno.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghybsbjmf.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/giialrrfc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxidilkaj.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gyxgufzkr.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gegejvknc.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gnhcjcgzt.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/groyufdhy.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gsdrpessw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gpiorrhjc.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gyugasziu.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gfxqihwlj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gmlqtsfdv.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/goxebmirb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gcqtnwjls.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/glytpjprp.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gnowidsxv.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gunnutjcv.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gkpgjqvyn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gosdtbend.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gagxdojky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gczozmdoe.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gyfdgtdsw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gsyamjhod.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gzfwijopf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gqorbyeed.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsbconiqn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gboobgsxh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gbwuxzpyy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/glnmpkxhq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/glzrgteok.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/ggrocsggi.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gbvkvboip.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gpqzxblqi.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gxlrgjnpm.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gwvrrwdza.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gimrhxvvd.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gvsgkhsvs.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gligkqbhz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gvphggxst.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gvsprfomd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gglootbmo.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ggkdepnaf.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gbqppuekn.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gqikudzwj.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gbhcynvxl.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqsivkhgg.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gymcywqjj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gxojkresw.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/ghugzyzcj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gyyitalzy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gzavpbfkj.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ggnkvwgrt.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/guqeacprv.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/glbxuvmby.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gxcjckydl.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/glnyfbiwt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gcgfthewb.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gcydumjdb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gqtisnadg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gbxgnnwaz.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gaszvglgv.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gtlwrcyyp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/goindlaon.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/ggbpeuucz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gjxkwfmdg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gzqfrqdru.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gkjvblsla.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/ggaduyeuy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gqquutzxe.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gfcffselk.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gbbexkgeh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gvhfoyxdv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gllzimtkw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gqbsmrfck.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gpdkvudcz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkkinqdlu.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gslfljdvi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxfexjhpk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gucjjvbso.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gteeggcug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gkemlexrs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ghujhzokn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gqhsfvopg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbgzlpxpj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gwhzvxizd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gnuakutcn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvtrvvjqu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gkpitddsi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ggbuozatw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gsalwmafa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gqzsmefza.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gyiezlgrv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gbserjmnh.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gewhthakp.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gowqtevvv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gquopbcul.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gmtldoqqz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/grdabsrdb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/geymczufw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gkbnbcvtv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gjflvksxv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gpcfksjjb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gjcfcsiey.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gyipxlsxp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gccjtueur.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/ggiopheli.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gddqtafzb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqppqwik.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gnlsmolze.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjdnvilrz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/grpezzgsr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/ghcmoduxx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gpfgqvkzk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gqknajhrq.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gomboqqzn.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/glpnywhjw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/ghpsbhvxm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gbamfvzkc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gccpdknrx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gilglppzg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gwkupewmw.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gnuhdvytv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gmacjorng.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gyvxgaajc.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gmfhmpanv.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gwvqvzruw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwyesxnfe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpvclgiqe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gkonctnao.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gafcsdzin.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gusdtlmqi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gqbpzogub.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gzvzcvjpm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gazpzcboa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gtmhqjmri.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gdpzjkgly.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gwnjvmodz.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/guvbsitoq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gpmtaoxiy.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/glvkjbhhi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gjdcgdmzx.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gvcjonhcy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnogzansk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gcaoblhkc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/glfugzhvk.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gccyhznpa.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gjhnoqwmy.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmwbsckin.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gwrotdubk.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gyhbpmmho.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gmzvvpcxj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/grrjdjhow.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gxdfhhkqt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gfkhudxks.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gstksmysz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gqvddzuyx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gtaqwdscb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/goxbscrwa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gzggixmdd.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gwrxxjeaa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gkrjrwqur.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gmwepgyga.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gsemcvarz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ggefgkwbr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gppfadnql.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gjmfzbbes.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/ghviioqsv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gknayxrgb.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnsqslkvs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gnlrwkgsh.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gxethfdzi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gymjwexoe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gymrvfgww.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gxsertpbq.sHtML


<!-- 参考信息 -->