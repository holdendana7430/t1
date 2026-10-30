代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhydfckc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gewstbpzr.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdoivortk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvwivtre.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrdeewit.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gkyahfvwa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gubdenfhb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/ghyfnmihb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfeuejoe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gjkeyqake.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcbquizp.sHtML

[K05] 深拷贝对象
来源：http://blog.fanxiaobao.xyz/Article/details/gjxswujom.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghplgvobq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfudqevk.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwawzpiun.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gfftchcsk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fanxiaobao.xyz/Article/details/gcyqwofnk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fanxiaobao.xyz/Article/details/gnbkgvfwd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwabqwfp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fanxiaobao.xyz/Article/details/gwdacohft.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fanxiaobao.xyz/Article/details/gedwaksbw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fanxiaobao.xyz/Article/details/gyetzdqeu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fanxiaobao.xyz/Article/details/gpgwehchn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gaksamzsr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdynnrsq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fanxiaobao.xyz/Article/details/gprqmacnu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbznepmi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycqqqdhv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gchzpzjsm.sHtML

[K07] 进制转换
来源：http://blog.fanxiaobao.xyz/Article/details/gvfkzgnvo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjlupiwr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhstxasv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gpmzgnchi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/godtunrjm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvfuadkz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaoowpag.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcyofkwo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/glkfnrffy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fanxiaobao.xyz/Article/details/guoujfbqe.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gztttrbnk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/goovvqsyg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfxqvywo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fanxiaobao.xyz/Article/details/ggzlbkuvg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/gxevjebvf.sHtML

Go:   encoding/gob
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhucuqxf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrbkudbr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcyvutpn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gctmgbrne.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkgojspo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcxjkthg.sHtML

[L01] 发送 GET 请求
来源：http://3g.fanxiaobao.xyz/Article/details/gotapglju.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fanxiaobao.xyz/Article/details/gwweeyebf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfzmhjam.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gvhpqtmdf.sHtML

TS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmavxdfwg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fanxiaobao.xyz/Article/details/gftvozins.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggajgxtbp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfagipvhw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmowjwaq.sHtML

[L02] 发送 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gckclzlhh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gznnklxak.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fanxiaobao.xyz/Article/details/gzdwbdmqn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gtlxwkglc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/goyixxiob.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gfmgqrbqu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnodvqga.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fanxiaobao.xyz/Article/details/glnxmywic.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqcckxyw.sHtML

[L03] 设置自定义请求头
来源：http://3g.fanxiaobao.xyz/Article/details/gdvowmmba.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigbnvojr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzyanmjk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fanxiaobao.xyz/Article/details/gzhtihtcl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/glufzjldz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggspmjbli.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gweujgbwx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzxbocsd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gorrichlh.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqradgzy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fanxiaobao.xyz/Article/details/gwyrwnkij.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlzqxpeb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawpbnrru.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/ghzazvlwo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdndihnkx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/gapnsiomt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gsxukmhie.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkerrgkcb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fanxiaobao.xyz/Article/details/gusuylgqm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeomrfaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgpacqhv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gywxfvggi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/geytobmzj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyfyhlda.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrorjblr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmbmmdhr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyncjwjv.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gfpbfzixo.sHtML

Py:   resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmkaflih.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fanxiaobao.xyz/Article/details/ghztieeaf.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gyfxtrkby.sHtML

TS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/geueyysuv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjxrqrdd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/gjbesjaxl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/gchvhvbdo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gxcwufqst.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvdfbyfw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghumlceol.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybjkhewy.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fanxiaobao.xyz/Article/details/grlayasuj.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwizajcf.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlsbhqyf.sHtML

Go:   resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqlassal.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fanxiaobao.xyz/Article/details/goyhhxruv.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjlroinc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnxptaer.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fanxiaobao.xyz/Article/details/glmpyllke.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/gbtqbrryu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmhlhytm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gdhuqlcrn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gnniwdewr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fanxiaobao.xyz/Article/details/gstqldrfz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmxbdkmn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gelmyuuov.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpsrgocwf.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fanxiaobao.xyz/Article/details/girtaazed.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjphtewou.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdtkjitjq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqjnhvij.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fanxiaobao.xyz/Article/details/glqiggwab.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbxfqthe.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmvuofxsq.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcfpnxtq.sHtML

Go:   os.Args[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmejqbjuk.sHtML

Ruby: ARGV
来源：http://baike.fanxiaobao.xyz/Article/details/gqlxnwrbz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpddgexp.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gptdpkscf.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/ghfrrdidb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvratuqws.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfrvtzjb.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/glmglybsa.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gypvcsypp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtoluqzx.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkzwdffo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gpazjfwfr.sHtML

[M03] 执行外部命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gofuuhzxl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gzzglybkn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gldksqkhn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gclvpcuoz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrwsyvpm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gaweidsqs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbueyqcz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fanxiaobao.xyz/Article/details/gygaawiae.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvplzrwyr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyvejyhp.sHtML

Py:   os.getcwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnesdebiy.sHtML

PHP:  getcwd();
来源：http://mobile.fanxiaobao.xyz/Article/details/gskujekuz.sHtML

JS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gchxcdpoh.sHtML

TS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqwtdbxo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxacqernt.sHtML

Go:   os.Getwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gjuullaye.sHtML

Ruby: Dir.pwd
来源：http://blog.fanxiaobao.xyz/Article/details/gudfcilnx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmistmir.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvixlsrxw.sHtML

Py:   sys.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaqrcxrn.sHtML

PHP:  exit(1);
来源：http://wap.fanxiaobao.xyz/Article/details/gdzbbbbcr.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gundtehoy.sHtML

TS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gchzktjkk.sHtML

Java: System.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gxaoazcsq.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkawzjhej.sHtML

Ruby: exit 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvwjiirxt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fanxiaobao.xyz/Article/details/gnfgngmqo.sHtML

[M06] 向标准错误输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkjkigelr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqndnbktq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gnadvdclu.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwauvcoar.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/giujszymr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaevltxq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizmpojmj.sHtML

Ruby: warn "err"
来源：http://baike.fanxiaobao.xyz/Article/details/gcwofbrvz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjgdkwbi.sHtML

[M07] 判断是否为主入口
来源：http://wap.fanxiaobao.xyz/Article/details/gpcphqnaa.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fanxiaobao.xyz/Article/details/grwlpqjwk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fanxiaobao.xyz/Article/details/gnpxjncpm.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gsisdbwls.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbnoibrk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/grgbvckuf.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloggbyao.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fanxiaobao.xyz/Article/details/gjjimzkyx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwkuphfq.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fanxiaobao.xyz/Article/details/guulrrhoy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmiufkpp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/gbuojujhl.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gnuroylxz.sHtML

TS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gqtnfbbra.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqepugfm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fanxiaobao.xyz/Article/details/getbcjnvk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fanxiaobao.xyz/Article/details/gfosuyqtq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuvjfpkg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfnrmoddx.sHtML

N. 数据结构与算法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywimtccs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grjslbolz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gbatpngaz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxevpeymm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/guvpkljxx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfnungxt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/ghexgwuvi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gobwpshax.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gchptprxn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfpgzffn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukjrcohe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquctbgwm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gbyqtvslt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqxglhjg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpomfrhe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxaevkto.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcshvzhge.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokhqbctj.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gaiuarkzh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gwockzoyh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrugouad.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gftccsuko.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fanxiaobao.xyz/Article/details/gzneckmki.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gkvwsjthf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkklbmky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtjrvtqo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/gjlegwjan.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fanxiaobao.xyz/Article/details/glpabnkis.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrleatkz.sHtML

[N04] 斐波那契数列
来源：http://wap.fanxiaobao.xyz/Article/details/gfbpjeowo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqoapbfav.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbvlvenhp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gwikficfp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfmqgbdf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxticvyl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfhxbdoa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gstowhoni.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gvrwocknu.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkgpwlug.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gxmyukqeg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdblgrzyy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjijrshz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosnxpwhl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fanxiaobao.xyz/Article/details/gaafalnid.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gigwzzyeh.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyupjhudj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gygkpsxdl.sHtML

[N06] 判断回文字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdtazfygc.sHtML

Py:   s == s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gnbewyckb.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gtuvjlbjp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghahlzubs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchkkxdv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsiztotu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gofztszpc.sHtML

Ruby: s == s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/glqlzmyqz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxzyubwk.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fanxiaobao.xyz/Article/details/geuplcniy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fanxiaobao.xyz/Article/details/gpocvatsp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrnvwhmn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcwjoziz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwlukebk.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gevszeppq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gejqusypv.sHtML

Ruby: // 手写 Hash
来源：http://wap.fanxiaobao.xyz/Article/details/guqcjtznh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gmxmabpzq.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/gartvkyvv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/geqchafof.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqthhvgj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsafdyke.sHtML

TS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gurlrvijy.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfapnkmuw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjaueseu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbjgaqgs.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gncohimch.sHtML

[N09] 栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltbipfjd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwuatoca.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofxhxifd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcnzqowg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukslnzan.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwccnfxp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyhlizyg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/glqignfgt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/gvnrjxnvz.sHtML

[N10] 链表节点定义
来源：http://3g.fanxiaobao.xyz/Article/details/gurarqwwy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fanxiaobao.xyz/Article/details/gkpclisod.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvbukwtvt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcdrjrup.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvnuentz.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzqtpotf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fanxiaobao.xyz/Article/details/gbmcpkomm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvqgoyjw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeyrkyqt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/glwcetckw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fanxiaobao.xyz/Article/details/gzzmxyvyy.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmljukfa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gtabkmmny.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/geryxsxga.sHtML

Java: // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbfniyay.sHtML

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gctxsexvy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/guiudwqtw.sHtML

C#:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gppdubzuj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fanxiaobao.xyz/Article/details/gqrthlszu.sHtML


<!-- 参考信息 -->