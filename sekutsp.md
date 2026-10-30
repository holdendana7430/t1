代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/glsxtmmwl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gglrxhwoa.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gbvtakxyn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gaitccvwp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gnqkjkcip.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gflmyxgsz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gyqfekagr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gvlskvdim.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gkptjztxm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gkuankvvf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gaihnmkwr.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gvmvehpxy.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gkbpojneu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gywxxklee.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/glttlsept.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gksypptvz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gymszeivm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gbmrjrsqm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gkbweouns.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gafrzmlmg.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gmbilxszj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gxdddyptm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/glsxaubuo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gomgtnhfi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gbaspbugz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/gjwxsyzbm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gdttdbgil.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gcphyjcyd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gmujasdhb.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/glaapdxnt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ghkofwcbq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gqyixrvab.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gcmxnyolt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ghdkvyqah.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gmiajhuwd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gcpqqubie.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gyjsxkymy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gpzeqlupg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gguqxdamh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggqcwcchj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/giazkglbw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gghdinidm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gvwzhpixb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gpyyeceyn.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/guajezkea.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gulwdlntp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gxombequo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfczkacuh.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gjiuspdee.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpqnodbtr.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/ghjhqazsd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gzpvbnkas.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gyazfltoj.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gduqocdor.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gtrbliqwp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gdnzdaxsh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gxtmbersa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/ghyhlynei.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gginvlzug.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gxuonffzu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gwafagzau.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/guzwrmnwy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gkadbupye.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gwmkwdsdx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gwltogodx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gqhinxueb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gksojxcgb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gmgerzvdw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/goinpxrts.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gygcvwmgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gasdtooyg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gvpjhmeys.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gksgripgd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gcocepxsz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gqeytazug.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gbxbvlzov.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gxztqzrpt.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gtreauvsy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gzydafbrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/ggqqxynsx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gwoyjnvay.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gfytevjhg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gwlcjsiii.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gbvtzzeqw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gkenclrap.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gsxiobger.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/ggmflxrvc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gtesaymyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gdliekwqi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gxrnjliys.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/ggdhedlsm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/guwqszvhe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gvgntprmk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gszheybdo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfbuqbqnw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gwjbacgxw.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gxbcvtetz.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/guevzjnil.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gefcdnnju.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gbumdjeyb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/giredqirc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gpbiixodx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gmbdgdqqt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/ggaqfbjpk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gnbzvrugn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gegnmgtsc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gtvsxbqtk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/glexgofmf.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gdpoewswr.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gtjkldsbr.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gmdkxxppc.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gaoqtedxy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gmungtvuo.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gnwxifbzo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gwjciqiiy.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gnwtktxmh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gecolmibd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gslldqhma.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gxgwvxdfr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gtldpilvo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gzbvhuufi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gswkbvnri.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gefypgejy.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gfyizteeg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcdfjlnhq.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gsuyybhhc.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gsajjdwyd.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/guzifwtkd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gastjvvxu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gngbujmeq.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/govdkbbwn.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gsayoidpc.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/glacxljgb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gnaltzlzv.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gvjqtabnl.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gnatrjlcw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gylpxjoic.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gxxgpemfl.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/geircncpk.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gcekxpcee.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gfisltaft.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gzbvrefrs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gbusjwioy.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/ggmaeuyti.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/glufzwtof.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gtkibzdjn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gbytfcjpi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gtpltywct.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gesxqqanl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gvlcfrmnp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/grjhdorxa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gvuiogasq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gxiorenni.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gbloscist.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/guovysmkn.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gihxvravn.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gvegibxtc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gzawffjaa.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gomofpbqf.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gxbtfjwkd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gpkrnpvsy.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gafanqexh.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gswdbfkcc.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gvtfwmshw.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbknvtyvh.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gfyquyudr.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grtuyxobf.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gabgqsrmg.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gxjzurxka.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gvwcubyhn.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gfcdgsyjh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gbctvwixn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/grzscbjur.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gehsijrbs.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/grmpnjequ.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/ggoqicvrd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gpkxhuyqw.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/glhdgtqyp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gmajbfndq.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gsehzsxhx.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gqwtgjjob.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/grrcjwwbw.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gxlzkodhf.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gjuusijrz.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/guvqybuzx.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gpfjixuwb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gjrspybvw.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/glmxtpobe.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gzlyrakgx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/geijjdwic.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gerrztnnl.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/glndjoszk.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvqykgl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/grsauwekk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gytjppqdn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gkdaizfbr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/ggnxfhayf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giaggjhdg.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gvmoztvjt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guwqlzmyp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/ghnulncbc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gavnvlcqo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gpcktlzpg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gehdlyhdh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gpvqcwbeq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gfmgixvsu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gujhqirbh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/grnzlbywn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/goayrbmqf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/glpvmihyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gwdwhgsgp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gtxnbxazz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ggwuqfnvj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gsvqdrpzw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gquthxukc.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gufbjpzkv.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gbhlfybrs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gvbxdphrd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gydbdwcdr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gwmpvizjl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gsbkmfkse.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gugzdvcyt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gowlnlixv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gpdwgwvdo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gsvqydddh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gtwxkdsxw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gevboculc.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/glcwyawgc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gndvcitfa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gnmsrgrac.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gdyjmqgrw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gvpmlpprc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gkzyfzjwk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/guarwiliy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gamxmmawz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjxahhxaq.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gvaiyiehn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gcnogcefs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/guzegohwp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gsevdetcf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqfrbgptz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/ghryxwiho.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/grigxjcgh.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gdyfrydhr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gwkvgjhho.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gixroceny.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/grfbydzgv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/ghzvgjtvw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gtspzqrmv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gpbgbmbca.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gharpxdma.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/guoardkjy.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ghamfseks.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gtcfxpyye.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gehxngqka.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gzuubguzv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gjsvuyuwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjnwwzzu.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gxbrdwkow.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gckrnkvjx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gfhvbktck.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/ggynzfieq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/glftjxjli.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gtshumofv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwqvrzeor.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gpcrplooh.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjldlsfhx.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gxdjygzji.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggxummilt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ggbzkqcxm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gsggfytea.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gleunygco.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/glqswhrcx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gotzkrruf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ghfbbwfrh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gaurtilxd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gydggvfxc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gkdurpukn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gecmjadsh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grjwacrpp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/goryenicu.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gonpzyjjh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gabfvtdci.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gmvuddhsb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gewwluynn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/ggimqqinl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gqdxssadt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gmwvooxnj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gpkbvksmo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gkdmzvvtl.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gsaklvfnr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/guawjajkz.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gzmdfxvne.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gynpjebpx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/ggpmojotj.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghluhiark.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gubbowiqg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gmpiknszk.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ghyegciio.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gxnxjoymb.sHtML


<!-- 参考信息 -->