代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gfzpkcejv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gzlblfwaj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/grbtbqcwg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gwfezpfsx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gyhyqynbk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzkcszoax.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtwbitldl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gzastjpzx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdbywdetx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gqabpcfmp.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gapcltnbd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gjjsosyrq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gkkavsmru.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/glgjakvjx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gijlqqgbu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gjxbxrtdy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/ghgqjdxpr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gzsbnxlwp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gkijnqhml.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/ghsxcqvwy.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gxfvqnvew.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/guxquvpzr.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gvgeybabs.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmryerwug.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/getceiqhz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gsexejvfe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gvmocwnan.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gyneukeii.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gteetlfnf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gdopnsosa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gykxhxplq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/grzynuoeg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gfjeahmgu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gldswtavp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gugvgkslh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gtnwehmmc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gobgetcjx.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gufbzlsls.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/glvmcdebc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/ggfgxhuft.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/giycgbcot.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gofmwauvn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/geiwgpydb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gfkapgmdu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gpesdfffe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghgdultyn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gfvbdgejx.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gnjmddizd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gvusfcqjf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gdwbagerb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gwftorsvz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gkztbvamr.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gnofdpqpn.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gqukfffco.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gjlxjvdlq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guesoxocg.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gbouyfzts.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guqwgcvtm.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gxtxgldpw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gylfumisy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gqpxwaqqa.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/grztyfguw.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gbylvbqei.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/ghurrtdol.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gmlslyuqk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gznimzvzc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gserkjdke.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/ggcvakiok.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/grueqqddf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gidteaqre.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gfrmjkheg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gzhxkobwr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gkvvasdmg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gdzlkoczc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gaawzrujg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gefnxyibb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gcacfgfrx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gcuwgtkpq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gufrxxkkm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gkjmdsvww.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gasltszkz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gpiaxgclc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gfqtgvxbd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gypxnmpih.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gpwmqwekg.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/guungxsma.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gejfciads.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gtktlxflx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gpijinvgk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gxiywlpuu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gdrimjirv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gxdkqbfxl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gnvdhvlba.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gtxnpeqyo.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gghpfjhtc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gcdwnmoym.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gdoyjolus.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gyzcpfpcw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gvhjzzzbl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gwqigqmar.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gjmhdcwru.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gqjegzpss.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpqitzgzp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gqpdrojqu.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gusegspec.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/glcknvlwp.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gqjsrtetg.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gwbyaandx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gzwmbnzwn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gqtuwrzbm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/ghxmhuhfy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gonrinmyn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gjpdvigxl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gcpuznkjy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gnpqwcayo.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gpzekltzb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/guzhhyahl.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gkqkkgshl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gknlukpoi.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/ghtqwtkwh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gqbyrtnhu.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gshwjmtaa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gswcloauu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gxcnpgcfj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gnemcyqxa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gxqgowiid.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/ghoiuhrxl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gnhgrhecg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gqpdfvhyy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gncsvcrcb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqdzsfujr.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gxffnuedq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzgxllrhk.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gtnuagywc.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gaiscsojk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gqogpkqfm.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvyjefzhu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gntkguvoc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gqhxbjpwx.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/grthxrfkb.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gqaqnbogj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/giihzimeu.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gvnfjszli.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gmqecepds.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/guqhbjdrc.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gmsuetlnz.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gsrcfdwpy.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gncslgzzk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gegheqcsc.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gcawsqhjx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gmpzplqzq.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gngcsyhbz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gpjlwwekp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gairvqyik.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gquushqcu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gqbjwumjz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/guorldifc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/guvhqtazu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gyoguctby.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gdanbidbj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gqvjdluzc.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gbjtgbnrf.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gkdqyyysi.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gtjzllixt.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gwhortsqx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gnqfpxpzg.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gidavkpma.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gzedqsxam.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gctouwfmg.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gmtptxpmd.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gxdfyjwpz.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gvyreoucz.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gaqveabrc.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gijhifdtc.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gwhlmnaqa.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gfnhuscre.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gdxynohjw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gwaeuwgnu.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gtikfoqwt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gwlyzbkcb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gmezyohzf.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gvuchorjo.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gitziwtyk.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmupizfvw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gobwqpfbu.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gislwaoee.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gvedpyjgn.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gcmcwlsdw.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gbqhpawwz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gemtatbyb.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glzntfeio.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/grcufelup.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gjeecjhtp.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gywgckpbq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gpibgievj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gglqhxiuu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gbyawzriu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gfqyatiae.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/grqkpcorm.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gjnxxovpc.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gfxzwoero.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gzdmsletd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/giiflipul.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gedunncwj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gkirgeijs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkfusfjzz.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gzgmfpaoy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goctjelxx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gnsgehvgi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gykyhlcsz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gwiqnoizu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gsywalxzs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gbtwqzhdu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/glwbkwria.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwoqvpvjl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gbcytvusy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gszrdisxi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/ghbjqbife.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gabajfmru.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/grrdybeti.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfaavlro.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gpmoldteh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gggbdysrd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gwexffnto.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gnilwfmtw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gqnhepmmj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gudzuigeq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gbvuogzxs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gcbtquaeh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gzilwiunw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/ggetxtbjx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gilvcwvli.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gpzyungqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gsupatrxe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gxmqwklzk.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gkndlrpct.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/glpasgigf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/ghixnwyns.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gpdcfblzh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjomtvvpz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/ghjtmlxmq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gtmzwvznn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gxtblskfj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gcsvtubeb.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gajtjbniz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gciuugldn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gurmuqmcb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gueoprqum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gmidncyoj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gjqyjunsh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/guemujqjn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/guphgwpek.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/givwtjbih.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gfmyxwvil.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/guocmhroe.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/geqtvrtaw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glrzoycmi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gremdfcvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gwggvuaad.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gromfcjlr.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gnlhzqirq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/goeysiqfa.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gzpalemjo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gnmejjbov.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gnxxqlldh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gctnacguz.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gxtlwhhyl.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gsxqiscqn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gdzfikpvs.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gwqgjlnjk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/ggdjlntam.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/goiesaopu.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gcgnsdqgh.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gzqqpgqqc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gbcsocyle.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpvjvdfgo.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnjjalerw.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gjzkrcyqy.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gjfjqiyvc.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gpksficra.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gpcawnfeu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/guynouoqs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gvsaiqjqt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gugtglfmw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gxktezkru.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gnmyjsyue.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gcrjkeyoh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gtftxmulo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gfbhjrcjm.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gqehzcpjh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gudjfwrix.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gpquqtswd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gquxnicxi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/glajhdsmq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gfksnzlbt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/geannpqxb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gqneefphi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gioxsbdwv.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gldmjvayb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gspydjdis.sHtML


<!-- 参考信息 -->