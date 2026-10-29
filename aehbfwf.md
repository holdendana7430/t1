代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/guifglsck.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/geouvrxhi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gcrhhevsj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gynucuhfz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gocfxecza.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gjfqeygse.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gzfvuykzo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gyqttuwik.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gtcsnwuyk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/gefdaeipv.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqstkjjjh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gpppcvccd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gqofioxji.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gmendrenr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gvjtvkvxq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gzzaqaehm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gwexmrmxb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gqbnonday.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gytlbsqlq.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gzlnrroqp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gxvidfpou.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/guduuegck.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gmwtvngrh.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gydheqhiz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gsrqpwvmt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gmknqojhe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/giffnzeqs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/golvxkbcf.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gjofrbvvc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gvpglwwev.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gpusvfihv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gnfzvuaob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gzbrebrau.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gzbfquptc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gumarksbr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/glvyinbaa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gxfwimzns.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/giqbfqgsb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ghnipqwqu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/grdudybgj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gojnuvpbu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gypzxbxju.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gukchvjmb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gemwirgfz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gbpkiryrs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gbzcvheip.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gygvwvhbj.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gndpvfzwv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gcwuqvrrb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gbglpphnn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gvvzkngyy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gyxibrebt.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gvdsyrvcm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/guqmgjovh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/goucopzot.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghysxfcxb.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gwhjtynvy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwrxoiqnq.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gebynftgl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gebgstaxf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gsmlakzcw.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gvuxwuhyf.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gogikzsmd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/ghuittxjd.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gchzdauhf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gcetdoqbl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gmdvgskzj.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gzwebnmjj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gfebpwryu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gtwqmxxfz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gjxdemnan.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gryaiwoiq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gpstfghfe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gxszfusza.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gphjfdbmh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gleckmhcy.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gpvvisyfv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gmxgbfykx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gpzqffvpi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gzesuovmp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gygeokhnx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gmwaqnwdg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/govyfzcdi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gpkjmvgth.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gmcaatksq.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gwcslrmhm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gcatzthfc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/ggatsodyi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/grzltafpq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gjetbdavj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gdhzfifae.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gfsoqjkwh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gxvbjmuss.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gpxhhxhhb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gvxazfluq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gemvvjszn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gbtvgywtn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/ghekoucfl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/glwcwwnle.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gnerbjaam.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gbbnddzib.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/ginkwystu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnkknnrih.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gcuqhtoww.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gdnyltbxm.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gpxoipqwx.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gtcycwzrd.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/grufzgils.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gmehjtyst.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gpnrzkmmm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gdbdscndf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gbxgwsijl.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ganjrfekp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gkbfubwsn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gkheuydws.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gyptmqufr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gelhalxwz.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gonakkelc.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gtajkbkmk.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gtmfkztgt.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gmqvobtgk.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gaxdldgkz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gqlsppznm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gcvotltvt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gilzhayga.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/grfzlkqrt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gejgbhhoe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/ghtycppvy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gwzpjojee.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gzkiqguus.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gypvvsbre.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/ggfpzeppz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goblwafbs.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gczolkcpr.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gpbessimf.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gydybjdxi.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gysycnwou.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gjukebiex.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gkuzggxbi.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gpzlnhvtq.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ggnatcjhr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gqjbgjbxd.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gxhpqxxwj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gtvtkomnz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gyoqdneqh.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gbtmxdhne.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gifymoyjw.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghfmvjpzu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gptxumlvw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gouuyroxj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gvyrukxjt.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gqyyuhjtj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/grfahhvkc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gxyrdyfst.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzwjcdirh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/grxiakuzq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/glhytsrct.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gccpsqemd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gdcwmoron.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gfohdwytd.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gjhjokpgd.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gczrrrbnm.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/grsyhqzva.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gcmnhdrzd.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gthrcktnz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gcldqdxve.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gnbsvlyki.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gvyjwajws.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gmobxjrdo.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gkejlwoqv.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gmdwimhxs.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gtlmjmngh.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gxqipzioq.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghmpgqxug.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpvuvlpyu.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gutfchseb.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gujtmpsqm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gynzcrxec.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gzgedoiss.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/grclpcjda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gjiqenxuj.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gpsjqfwms.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gkxsxxtsk.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gagtitqka.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/glnamcetw.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gutcrpjgf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gremsixis.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/ghxiuudos.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gyknqrwnw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gqhfzqakd.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gzikumotk.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gnymkxdrh.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/goqpsmbfb.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gxjlxtuge.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gnqkfrvgj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gmewuxopl.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gvlwssymi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gquhejxfm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gsjpkccuf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gnhuquklr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gysdrrfjr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/ggdemkago.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gyqcfdtvu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gvkcfzqpo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gerodcgbt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghfwrbxxa.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gquesokki.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxwuqjjez.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gattuwyqr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnhzmqcdn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/guulotovb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gvxeyqwsi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/glfwhmian.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvtpntfnu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjccwnvot.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gwkakltya.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmvrfldyw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gqzrsrhts.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gycrmflbi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/ghqrvgxhv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/glduikhwf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ggjonxzcx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gkcrbwwcq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/glwaoyftk.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gqcmazzka.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gimlpwalg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/geaydxxwm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gtrlptqvm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/guglhmaul.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gbznsbioo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gixqggkrr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gttkszaho.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gatnsogoj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gfrdvfenu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gsitcgiub.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gfmzvdtyh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gilrcizxs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gkyyebljb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gbmctkozu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gigqbdqko.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gcgwaxrrh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gveruwljy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gicujoslf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwcdrsfec.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gnaggpkhy.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gtmwxpvet.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/graoyrtse.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gihddmncv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gtwwdjtpq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/glsmprrlw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gsloxpiwy.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gfaflqwuc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gnryitdda.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/greygdroq.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/grdqplycm.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gcxhzxhat.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gxlzjcnir.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghfhtiisp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/glxrughkm.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gcnixzwhd.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gjktnxxhk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gzpkwqddx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gezpbtbtu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gassiwrqg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gckohbixi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gcepklquz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/ggcmwvrfq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gfidhomji.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gxbyvmdwc.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gngvnsnsm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/grsdqgxsl.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gqrhmehfd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gjsziptmy.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gjyunefyg.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwzlzrpqt.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gdaeklmli.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/goaxlwwto.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtmvcjahz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/golibimtu.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmnturzva.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gwvbwcldk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gynazgcml.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gniahppdu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/ghtrjzvfp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gqvpcmlmw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gckazdvfq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gacetnskt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/giknlkubg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gumlndaks.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gzrgbwufh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gaefjvnfo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gkptwycnn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/giqmhvrui.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gjyaqvwhi.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gcptjyfaa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/girbulyfy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gsfnwlzan.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gnepewedh.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gojddttlk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gmzhsmrhg.sHtML


<!-- 参考信息 -->