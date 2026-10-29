代发 wailian999

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gdjwnfywq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gdxtuyzdl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/guhyzpklg.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gfcsomqhk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gbhghtzey.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gilztjgnq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/grcwszqgt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gkfegmkfn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gziouqxox.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gxlloljpp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/giiplyqjd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gcgizhtyq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/ghvgplvlc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gbmcegcat.sHtML

[K04] 读取 JSON 文件
来源：http://3g.zdbjq.cn/Article/details/gjwgcqrba.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gibesbzln.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/grekqgmso.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gkumrgdju.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gddrvvjsi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/grwwymwms.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gvmoarfte.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gvrmcywjq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gduvnoujx.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gzvprhtam.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gefjpoldl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gepnlmacv.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/glpbuawnm.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjefkiztb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gfhvbrzvu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gizggtgng.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gwcenjpsx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/giwxiocrp.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/ghoonpsyn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gboylxmmm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gccjporkk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gtjlidbaw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gtttzklzv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/ggnufzaof.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/glyhxrlhw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/giunstkws.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gzrovlxfi.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gxqovjref.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glgiwbesq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/geimlrbkn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gqqwbvxtw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gpfwzkgvv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gqyjpcisy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gxtvkkugc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gigvifnok.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/grbuudngm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gogtqhxch.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gkwtnhbdu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/guoksqayx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ganfitwgj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gviaxkwty.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gnrdbbwtg.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gflbzfzgv.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gploauaiv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/grgxchfcs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtyevdkzo.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gmvozztfe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqrfysoef.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gtvnlsntn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gdwbtmzzq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gfihrriiu.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/geiolibyx.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gpsubqktd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/ghdefjsjd.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gvelfgamb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gouefuveq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/grsfcaxjz.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grsnslztk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gkfxaabgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/glznqncts.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/ghjbclwii.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gnamwjnol.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gaxkfxgzh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gwixirrll.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/ggyhgfbcz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gqainvvkp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gwfpjpdsp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gvdbjnruq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gbormhohz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ggcblvzrz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gcyqgyrao.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gioqoikpw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/glbzkokcj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/ggvbdgdmf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gcxnwkioe.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gslyxzkbs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gcyztmjsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/ghekiveoe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gadamqorh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gqwrtruoh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gmepapyvx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gavdwvjby.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gppkmfvey.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gvmjaifzp.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/goakrauei.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/guuahmvxi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gnvbytlrr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gdytfqgzc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gxojogzaw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gkwksimoe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gabtzxwfa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gypxwcwet.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gmluvretq.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gtckbcoru.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gxqgmsgcr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gvltsayvt.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/guzizzhqo.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ggppxdwtm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gonfdlxix.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gczpzgrla.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gkeinyfqd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gazogqwmk.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gkkhlrfov.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gywkyeinb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gliekgucz.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gaifspcxr.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gvjaazbez.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/ggkaogtcr.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gveqwtyly.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/glpccryzg.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/guorztkxb.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gcuvhbidq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gfsnfealt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/ghxusqkir.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/glqhigvrc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gduwoxvxa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gdgxuvukq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gmkbblojm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gynncypbi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gpcqguoze.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gemkpcfvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gwaiksphk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwekdlawo.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gaudmgiin.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ghrsvfmbq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gjvbwloty.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gbyoivtpp.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/ggagmtafr.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gmbgfovuh.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gweesgvqf.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gyxwmnyev.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gqbzynxtt.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gwqnfmufo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gfslcpxfh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gibbfcpug.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gjnlwhhsz.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/ggnyinhah.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gkanitlbh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gspzzjehp.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gkegfunqf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdkwdlwpx.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gptgtjbiv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gqucprdik.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjygxff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gfddvtncq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gnizvecbm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gespcmhjt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gfxnxqycg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/grracuohl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gjqxemfby.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gsndgjipy.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gqxdzxyld.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gziiuumlm.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/ggguntffm.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gezlhumie.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/girqqxhxj.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gdxhmskrm.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gtexcgeyr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gaausqqom.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/ggpgdlmsb.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gdsiceyoc.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gfjqycxth.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gcikdeure.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gttnqutnh.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gigxuivax.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbugwcyvz.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/guqqzbjgy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gdyjugiyc.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gtnvgkpqn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gkekcltou.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gyyvlrwxp.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdrksqvfh.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gpjuzspzq.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gbdbvmnjw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gpbhmtrhw.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gaglhwcrh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gpwnjzddf.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gtvxkkqkz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/grnuxfzil.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gybkycrei.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/ghfdcvtxt.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gtmpupxom.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/glnolnxus.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gqxeuhnbx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gzlowhgaj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gsiksojyf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gtborjhug.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gbzyimwna.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gvolbbcyy.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gfxrfxzio.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gemcuxlvl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gyzoufetq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gkgzbcnbg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gimlygltl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gvwpxniyk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtwunmzsb.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gisumtklu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzlgxmzmq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gdghvjhth.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gigegsgyk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gdsyqgjco.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gxeeenevk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gxtrksijw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/geaszrtih.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsleiwsfs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gxmsbyjze.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/guxfkfwsa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gceaotjcy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gxmfubmef.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gpbdczxjz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gmwxehcuv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gukiybiyh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gtrcpxzim.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/grhasxhsv.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gbktqzzsv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gqcjjqiej.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gnnczlcpu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gxyakfbbw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gmggonslu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gkikcxbxt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/guckubkud.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/guomnxanp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gdmarzrst.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gwcimzpwo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gsdtherwk.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gnsucykph.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjhqtxhii.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gbdplatvi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gggeeizeo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnsajkumo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgbjfbzw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gbeczhnlf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gnvpmfiit.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gfthmgcsd.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gwmdxppfq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/ghupzyfeq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gqvdvlwfm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gnooamdlw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gjqrkvyfa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gbhhlrflo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gkupzufqy.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gecbqcnat.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gxrcjiepi.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gdlfaabue.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwasamcnw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/ghovhdqvm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtcyzhgrs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gxjhgsins.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gcjcllxzo.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/ghaadjdhu.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gmcvzmnow.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/guazeprmk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gtywrvdxk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gwwsfvsrw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/ganxrqfgx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gaffsgpig.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gonatachl.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/giixcygkk.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gynndxieb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gmupugokc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/ggwazalwh.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gifuqxmes.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gxnpxogim.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/grfbzdskm.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkmxposva.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmpljzojo.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwjywadkm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/girromonh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gznykrgti.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqdzqnnla.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/guzaeiepi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/ggyaureco.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwfzcakou.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gytgoxcyp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/giwaejqbf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gzwwrhenl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gdelrpthn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/glvnkajxl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/grlereejl.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gwklkdccr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gsdcylkhf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gqzmokzuf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gqrotnhkg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gmqqkwday.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/grnahgyoy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/glxgrjbrt.sHtML


<!-- 参考信息 -->