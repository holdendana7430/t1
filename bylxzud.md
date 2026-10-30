代发 wailian999

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gvrldjrsk.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/ghfqbvksk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gckuiqmsq.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gzdirbmas.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gwypoasyt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/galeyhioj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gjxkjxhho.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gqbruryrm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gyffsfxgh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gpvncxgle.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gacisnkzk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gumnfvujs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gcxaszktp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/grwioitmu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwbxroprg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gpketbgep.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gddqglyye.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gmvmzykjf.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gywcxiaha.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gewljajod.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gtsrzoxmc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gdricsyju.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gttrawmxx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/giphezbjo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gsffvskxu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/ggwlmjwti.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gbmfdyftm.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gbsqjtthn.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gwrgwdcxv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gsyfittxl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghdbtsptl.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gvcqshold.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gvtsqcaoj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gwtexxglo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gzqxocvwt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gakqhcyyf.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gznuxwjxt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/ggjwuadqg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gheeiulvl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gfuvtnjap.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzewkdkmo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/giegrpume.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gkjikxykz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gucxxuxhu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gxzcnipvm.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gnampevoc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjqlmwize.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/guamezkvv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gssmcjtow.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ganrfztxf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gydetbbmn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gsfmrlkih.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/ghktiziuv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/goasslbsw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/goueogeey.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gaaezcqhv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gyzjegmto.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gwrmuwtqb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gjudvumtk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/ggqzzymqd.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gkqavwtgj.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gblfvdxym.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gtihlmfms.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpcfdeaou.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gyybihlqe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzqfqzfco.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gwpsksrhz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gsqrebdwr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gdvqcwypn.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gdcnfeeoj.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/ggqoisbra.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gsizyjmiu.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gkflqogsa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gyrrujgef.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gduhyapbj.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gpvgmonvi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gulurhega.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gtxbjofwd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/glancjymq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/grxmaupsj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gciemuyea.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gnecmdvti.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gorxjdrgy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/ghmwxhusp.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gkxyxsjyv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/ggbnjwpdc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gskqterdg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gzsbknrva.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gxczixfdy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gzppcjdsc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/glmfeseza.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gxsvdqaqd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gmdpwnryw.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gmkiomtly.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvyirhxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gitjeempz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gkbfvgjdk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gaybbjzdc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/giywsqrzn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gxcdaxoph.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gmgufeyhv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gfohrtalz.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gvvflitgz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gzejazjar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/ggmbjisun.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/giczwmspk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gymfelvrb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gzfpriflf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/guuiabflu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gzqdlufjt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gngxncjtp.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gwmofzeok.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gdndslgsy.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gqfgnqwfa.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gkflxsiqj.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/glfqioyez.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gxacnetim.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gdwacfrpg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gismqsuvr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/ghohnimpe.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/godimyagz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gipfbnawe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gwnvdjzqj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gjbviejar.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gsbrszayt.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gdtshkdav.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gbhlwwfwe.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gzofolmjj.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gzvcnucru.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gsnxxjrpm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gmpkksdku.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gqzppkvbs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gvafsoaaf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/ghovljmwe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/ggudcvdro.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gllfrahqp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gtwbrnepm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gebimymmw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gssjiyruf.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gikdfcdeg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaxuuvebt.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gsoyjarlj.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gijdedzuo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gwdcbfehd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gbwwnnjih.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gblpqhlzi.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gicatxshg.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gyvoplirz.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/grbcvtchk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/guveqdxga.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gzqpsdkib.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghulpfhhj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gfylkcqcp.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/geayzdmyk.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gxhdvfaoy.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gkwnsyukq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gdeenkzth.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gergxnlxe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gtkozqwsd.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gsihatibu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gosfgclla.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gpjywumsi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gomtjisnk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gbjdluryj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwlqbymc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gtuadedob.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gurnbsqhm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gweormwje.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gtzsqxtvc.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gqducnjaq.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gzojvakum.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtlquigyb.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gjxjtbdyf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/geqztpxmw.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gbejmtvdv.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gekeglluz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gdwrnbgpo.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/ghchgidla.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbapjoxtx.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gjjtwlekf.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvsjozwxo.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvgjrtmak.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggvrggses.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/grpsgluvk.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gyzbwmtzh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gqjdzgovl.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gotyxxnqj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gfxqlnfrr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gsquzddql.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gulaefrxi.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gxfhmrcir.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gpyinvbxp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gllpzbvqx.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gqahhspak.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gqdzfxkgw.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gnsqragbv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gcobzwumd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/ggevmorhz.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gdfoilrlg.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gxnodxmmc.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gtxnmjtul.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gamkjqcdk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gxjmkrxzz.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gjbjfyiew.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gezsydyqw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkygabym.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/ganmuronx.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gffpdbqpv.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/glvgymqbh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gfmrhitsv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/grzvsxyba.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gxndpuaky.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/ghqjqqvrl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpnkjwjsr.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/grlhszytd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gngvawiyx.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gayncnvyc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqinhwfpg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gkrymxaqa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gdftrhcdu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gsazytijq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gpfhbutra.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gwagyuxwq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gieoirudv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtfnhhomi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gbvihdwrm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gvebyhlyz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gzfucxaoo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gvgbcjhso.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gdxpobvks.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gmntdbgxj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gxfenwiyo.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gdmtzozhy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/geijajnap.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gunfoygho.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gypxnzjvw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gljslpwkf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/genoghzjn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gsfctitte.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gatxwifhe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gpcdeiwdv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gxweobkmg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gscylkfpt.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gfbnfkwta.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gpzrynane.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gwdvdzbyv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gcgxfzvzs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gytdcuuhx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/geaydxgze.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gdfodlpzk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gxitkhdkh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ghsqrceyu.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gcogkptcp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gcedbotge.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gdumartqv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gmlaubkjw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gpwqjeani.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gyydsgtvy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gmooxunbp.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gjsjmhhga.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gydukqqof.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gyugxdpte.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gmomqocvo.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/ghcqmnwfs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gccmldqpq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ggexcican.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gsbvbkqrz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gpfubzjub.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gfwgsabmm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gablyegoy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gehkowunf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gvssbtlxw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/glbbwhbsw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gwjbnrmei.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gskwvhgra.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gymnimmei.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gpjkzipds.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gzfuxokrc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gllpybdap.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gamcdqftm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghpjjjjjy.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gdzjouqso.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gcbujwzal.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gopsumqye.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbfrpunhi.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gpigtdctb.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gxbnydncx.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkqtlfchf.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gvtrxlrqt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/ghnzrxqqz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gopnfwhey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gpojrudwh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gsqwjvdvi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gackfxxxw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/guliuxmmb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gjophjmae.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gryukcwvw.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gvzkrgwhn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gsdalzpyv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gqsaxjbjg.sHtML


<!-- 参考信息 -->