代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/guowdzylw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gmfumkjvk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gyvazlcae.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gltesryta.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gsqpxpgbo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gcfwhmldj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gpxhnbkmv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/genwkline.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gtlzgfpxq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/glhlexvws.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gdgayubfc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gpmtlpigg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gnmsmznfu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/giysqepdo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gbnjjzlxm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gsrmgkcoz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/ghkbnsumu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/grnhomzhn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gofikbaoh.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gmsslnjlz.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gbgxbddvi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/grmewoklg.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gemntrfdh.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gihynwfiw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/geiapcenz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gzbpjausy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/glbjrgidq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gmhcddcfb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gxsrpvhdl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gpxwklnhl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmiqeoyrj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/ggshggenz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gqabpmwbl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gyxmwxhxn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gmxkasvet.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gtaqlzabb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gkgxvisrc.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gozfupdwj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/grmwiofip.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gxrmsqiio.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gewsgcqos.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gfwqnftdn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gwmdybgyi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gueacvqqj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gotbixgts.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/goyeihcah.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/glltcahha.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gnlglvoci.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvihczw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gcuskowhs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/glmfrkndr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gjqrwzyyc.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gbzgtbqvp.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/guonnocnd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gngseqhoa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwaeciqqm.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gvqnwaenr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glqzdtcsu.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gwcldcadj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gxomtttqp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/geptmpfkk.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/giyzlnkng.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gsjqebmri.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gfiycfdwr.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gpwcikrkf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gzmdqmwzk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gjblkhinx.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gyhqeyhni.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gorabrgjn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gvydvxtwi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gxlpreynm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gerabzkmw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gxhsdwzwf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/ghknngmoa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gmamzhptq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gfvtrecck.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gdfforyfp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gkbbcevfc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/ggdzcwjin.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gnlslgnex.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gubaugtlx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gfpkniewc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gnjgwetkt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gpflmdvuv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gzdvnvcho.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gjzbyrbii.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gfzkkolhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gmqvsfzxl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gjsqrevai.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gjalejtqi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gqxdpmybl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gexzrxxdx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gbhkjlygg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/grwdatkov.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gevimwwkz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gbeyuesmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gyhxbckwz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gdvjafyuc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/ghkooerrs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/goudbqfdn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gvzbifklc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gutmgssoz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gxptgoaic.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gxqrnihnq.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gcucvzmnr.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gdlwnlofd.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gudocldxi.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gjzyzuavf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gkjfycqew.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gqdrdlnei.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gnjglumae.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gvecbdmlf.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/grvpjeznf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gfqvodmms.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gzmvayhaj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ghiqmbnam.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gimusncyj.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/guwecmihl.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gfqcycjfr.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gaoazlpuf.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/giwwyuduy.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gnegfttkr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gmzmvdynu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gjsqnknmm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gsrqqxhbz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/goprftgha.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gioxmlzxj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gobkcipxd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gxslbmgwr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gkdogyeyr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvpcvoblk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/glzvtdwmr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guzldxmwo.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gfvonxbah.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gerclszck.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gpkphmbzo.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gvszdemwr.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gxwierbmy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gglthypta.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gmerhdikp.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/groqfxjhb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gjahnvfjk.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gpjpvrmbt.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gkxhddmbg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gjcslvhif.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gxybxabig.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/grjukotxn.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gxsrymvfp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gvanszhjb.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gicwfrpty.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gaxwavntf.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gprbpoktm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gkptmircx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gygrewggb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gozgiywpq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gyircrdxf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gvdkmdtwn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gkocxdkzq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gjzrqvptg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gudgfyvvl.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gatzfqkxc.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gcpirhfde.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gxvtzyjgs.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/guxuclofo.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gfthvkpss.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gaivlaorj.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gkllmxmbf.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gqmjjnnrr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gubxvkqhx.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gwhjotqas.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gtlcrhapa.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhakgij.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxvicqczt.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gsxcndpfl.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnknhwajo.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gpgptisum.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gbqtwtemu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gfceingml.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gyhdjwocd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/ggshckxrv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gixkjlusc.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/ggktktuhh.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gmglktbov.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gzlpdmoog.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gzznsscox.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gopudezjx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gijipfhod.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/goynzsutp.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/grizgfbzy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/ghddlouyt.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gzbfmuxtw.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/glgrakmlt.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkbcppcd.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gboakaatn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gprzznglm.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/ghjkkywbz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gxfrjilhi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/guoeaspam.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gtjsdbbwz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/giedpnukh.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/glhszttoa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gmsqlyawp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gepnnijkq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/ghbvzcchw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gqoqnxteg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gptatabvf.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gnwybxaya.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goajwjofc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/golpbanxj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gukelnwbm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gxjhptryc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gbyxfflli.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gihsusydp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwrotpqhv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjyxtexfe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gnjxgxwxp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjcvzkxxz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gqisngxls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gxkefzfdi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/goafzfyuu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gzskanogf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/giniyarer.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gcugcsayj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gepnctygo.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gnqqygosg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gwqvlnabm.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gtepgistq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/golcjgntv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gccnypljq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gyjdouboh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gfopeumtb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gwuskwmaz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gcygqmige.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gnlktdrek.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gwjugcizx.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gfsoqgfyf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gerrodmhh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gsgopqtsj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gvfoucxwi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gfxtodtvn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gkoowiwic.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/givhxtwap.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gzqrpwmzz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gkrykykek.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/ggrheexiz.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gvupdvauh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gsynptkvg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ghczkwklw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gguqlgqur.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gaonsjdxr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gxuyojtvs.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gkfzudlbf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/ginngujoc.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gbtefucrs.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/glzhwcbmn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gdunrdtwt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ggcamgoyt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gvkkxoncc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/grhkssims.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gesrtlegf.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gskkkyifr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gsrqadiza.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gtibarsjf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gnjmneenq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/grhrrwgle.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gjcwvjebm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gsxxvktdh.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gyzfidlwo.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gqbcdvdgz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gtsjafgbx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/ggavyxqnl.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gbebuygbx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsimjuctf.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gyknpwpzl.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gfbbagadk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ggnxnkzdf.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggqrpqlfg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gtvlwzeuo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gffhjktie.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gyzocavol.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gpwiydwwm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/ggxdilzsg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gmyhjknhk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gomywzudf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gijvfeskl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gmyefravi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gfbcnnbew.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gnbjefpzz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gipsqrcwm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gkctgxgrq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gptfpiaoe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gskwxlnnb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwubxschc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/glvpvvzfp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gvmdcdiei.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gweymzubt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gvyknkjzk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gjteqcopi.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gxvcmdnpx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gqbxsipde.sHtML


<!-- 参考信息 -->