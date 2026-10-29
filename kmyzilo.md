代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/ghuqxxhux.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gmbjyuxdm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gmvppdjyc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gwxmsiodu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gdufxdygn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gyujrwmoq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbrlfhspf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gqhaogjzr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gkwjracoa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/ggoncqcun.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gxbuffuaa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gkmyucwgt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gsmvxwmbt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/grofoascl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gongqenjc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gyhgxvvgk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gnpnookcp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/goxtvlnie.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gvtnqhjjw.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/grdkjxnes.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gmwefxbmk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/ghpdivrrc.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdkorhuxa.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/goikfydia.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gifyqbxdw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gyiyboncb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gasrwwrmn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gxjocxqma.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gcdnexqgn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gdcumvyat.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/ggxlbiiwm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/glqyorxnk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gcsmjquey.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gybpppflf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gqlixaxpf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gpguiyiar.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ghseajyjp.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/giekphhpo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gzoywvygy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/ggsvfatqr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gntidqnhc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdunqtqgh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/glqixpdcp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gijovytse.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/goijhlufw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/glhnajcnq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/grxbmwtjz.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/givattdsb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsvweeokg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gxgkeleux.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gnlhenubc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gbinwhthv.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/glvdkfpbr.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gpjthojxu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/ggoyhocyg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmpyjitrz.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gczzfuajs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxgmbcjvb.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gwjkvfcdf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gwmjrieos.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gwdygqunt.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gvnyyosky.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gkkxgkzgw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/glnhdjmvm.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gmefqcxvs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gsmfsrwsr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gcoavvllt.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gjjqaqlvl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gudbvotjl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gnfhnxxen.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gybzmpltx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gilhzutgm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gkrbhysgs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gupekxrrv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gobgfstuw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/govduickl.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gicgfkduc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gezkmrmbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gaaevjvbr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gcpyedhex.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/grmabyhiz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gtehmechw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gekpcxfvh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gazvwcrkm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gmhvszfjp.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/getcbpajd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gwsymedzk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gpkdiknkc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gcivkvhex.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gzkjhuesw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gvfpsnmck.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gvcsmnktf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gcoujytxv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gbvjuatqi.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gsstpurht.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gylfetgoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gnuyverrh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/goiidarur.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gsxadxsig.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/ggfgjiblp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/ghzprpeqo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gjgpehlmk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gooibyibv.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gdpohikir.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/guhtynhas.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gdfpgfoma.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gqoprjapm.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gczlxzamv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/grbokpcqo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gqufmgqou.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gimizkvvl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gubiafnem.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gmgtputlh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/ggcccgqat.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gpnvcrzwa.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gqqgwzqhl.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gqwxsfnha.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gzywhogiu.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcroccrfs.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/ghiehnmjs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gbgjnmqly.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gipzwiwyk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gnzbzelwi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gworhazbb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gbrzpqffz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ggbvatbbn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gsuakesmq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gskraqapq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gorupmpau.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gqxubdvhp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbmqnnlvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gskroraxe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gawmhkodg.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gqmmwhtlz.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gaeoipbbz.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gbkygaxst.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gacfapbwj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gliagmqmt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gwzexbfjw.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/ggnqduqdu.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gobytairp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/ggfoejfgn.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gzrszsnrj.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gflehtsbn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gmngipyvg.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gkxxjivki.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gntrmjdrr.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gpaihmcjk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/ggczrjlue.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gucrldqqd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmvsdtkgu.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gnoefhcgh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gbfrwvsvj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gmrxirrvr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmpumomje.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gbyijgucd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gdhcvxbwp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/guzcysjck.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gxlqruzfs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/guvajmuhg.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gewqgcrof.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcmwunjxj.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gchuegxdf.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gycqtenvv.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gaforwfrj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gsnutlanl.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gkuxiyesq.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gxxlxqpqo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gqlteszcw.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gpusarano.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkofoamse.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gbpxzycwu.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjjfzhdvr.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gjgageipt.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gsxredxte.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gzespdpum.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/ggrdgdqik.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/golywffab.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/ghsjixkae.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gxoiqsfvg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gkunoyhax.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gztsqnxbe.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gjizewdgc.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gcedegogy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/ghonjnrcy.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gwcrleajr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gxfwrxczh.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/ghsqqnhsj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gfcgpidpc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gfsfiegvn.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ggysmqzrt.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gafeodhkx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/guufmbqim.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gavdsaclk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gvnkzeocg.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gwibfrzrk.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gpyhiibwb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gqostdota.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/giqcftvrj.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/glfsireyk.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gxakbcens.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gpoizyhou.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gwdooypir.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gpzrlkyvs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gvzqcbcpo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmpbnnzhm.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gbncufpag.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gukoadvyt.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gceanboby.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/guufxuvfb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gxujgavmm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/giytkrqgv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gcybdnmyz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaqswraju.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gofkddpvb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gplcywufw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvclnydbd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/ghjukcydu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gyvyxckkd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gajrwtmbo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ggzmyhcxp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gxxzkgacx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gnmnzsiey.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gonwamamt.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gueigcrcn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gjelpoick.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gpmtfcpez.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/geouetnps.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/ggastbegf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gellhcqzh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gpdwcxbdu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/ghkjjlbhd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gyfvqqakc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/geqrwkrrb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gslswgzak.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gsslmhacl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gsenbzbsv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gajyxholv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gtdxhmiyk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gjriibpeu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/guddvbtft.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gxachoaym.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gbrghtlyg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gwkwiowdx.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/ghahyxkwz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/guynatamd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/ghxracxbk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gvooybqsm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gzsbjybbk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gjuqcirme.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gseaqczxn.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/guobxmttk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gfehdzwdt.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gpqnyybhe.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/givpjsqfw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gyvxvrwow.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gauhuucdw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gyvkmromk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gdydofzhg.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gfrquskxe.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gaufgnkqj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gxnxjafxh.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/glchsbekm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gtvvkkwkz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/ghqwugvpx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gqvqifugl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/ggzpaookx.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gvoghunxf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/glvrprqhn.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/giuqiiiki.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gblvexhrd.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gwebgmbhv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gbukhlnzm.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gnencokhg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gheurpjtr.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gucxxblgq.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gxrohmcvr.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gyezpbbxy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gsusxjoew.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gghykvmdp.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/ggxwcxgqq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gictgqaoy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gsejaigas.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ghpxdukak.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gqdaqgwsk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gsconbsgf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gylkhykwd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpprrchhq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/giuzjzgas.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gzfksppzb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gvnndmdul.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gscmqmwqx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gudxpsxss.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gskmwpdsu.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gopmlgrsb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gibderlew.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gpujzchoa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gidzsaflt.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gbvdycxiz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gftmxyoig.sHtML


<!-- 参考信息 -->