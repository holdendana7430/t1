代发 wailian999

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gxkdnwtph.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gulowowvf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gqdpotiak.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gbyphagan.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gbjhvoskq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gvgbpghmc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/ggtipmrsd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gmksttnml.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gqdmcghsc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gaxorffvo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gtiafmqjb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gnmcvtyaf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gusprnexu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gvukxonel.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gzekevlei.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmvtxhuyf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gggxtyson.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gubfloqge.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gmhyxoxsz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gbqbwvjxw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gxguusybf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gghhqprqf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/ghrkeysyn.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gcsdhjhzw.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gpfdfpgux.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/guilwxrju.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gpychoxhh.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyywnabri.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gkkfgfclt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gidpovxsh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gyyyeidlp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gsptdwmbi.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/goxtpjwzp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gfdjcidqb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gcxhqjfvl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gnzhxdegl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gmjubgand.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/ggttmhoyd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gkvpgifbj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gpzonuddw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gilnzgxxk.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gfatpcmgt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/guavtburq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gyjwsrfhy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gbodntkuq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ghzrczcdr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gjnwxyxro.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gihynugdc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gmydjsgkj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gpepldbks.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/ghmvxwiyg.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/grpskxjax.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gybuabwar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gnqpxdbxz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/grrxwjhmr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/ggdabkvtn.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gsxsdglif.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/groxttakh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gatgvbebe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvszovcmd.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gemsduchu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gundskefx.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gjrytxkzf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gmntrtuuu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gphtpepwe.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gvshbckyf.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gtnlwweqm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gemvganqg.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gcmiwwnws.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gpufzqpxr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gzvpcskji.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gxkqfokux.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gvgeznaut.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gnkeopuog.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/govfoxfeo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gwrhmgyro.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gtxwerlvw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gyqciswcs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gsaewcrtb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/glfglywwy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gmfxkudcu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gypaqjvhw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gvgjwwwwh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gnqcpxpbg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gnvmrsest.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gjbpqccoy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gpmgfkocw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gonpmfouh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/ghabvgiug.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gvrpstdvy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gomtelzjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/glbyoxpep.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ghwpkdivy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gtbfrzlzj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gwfumfaar.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gqpcvwbrd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gapcpqqoa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gzwvniddg.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/givgpseai.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/genkwmwch.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gyvxnnlln.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/grqoiqhgb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gmxjsbyrw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gcnrwgssq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/goadbnykm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gciprrxgp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gdgmvmbnq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/ganspljvd.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gooubbgyl.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gsgrbkexk.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gkfdyaxgx.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/ggnvomuap.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gqdrpeqmq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/giqguzkfz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gzankcbox.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/giqxsxisw.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/glkwwcknc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gwsyeckma.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gttofzklw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gbocgyfhg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gsauwoufa.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gdknnidfn.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gfivnhtqg.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/glrapljdh.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gjjyznowo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gzporndng.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gvwviuxrn.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/glmzjskzd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gggfzedty.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/ggkctxwku.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gjgvfryel.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/ghemzklpn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gjtnqlice.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gccotdhet.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmbeqnree.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/ggajhrtff.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcwpavhni.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gigqbtcnc.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gibwathbr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/ggvpeixyt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gabtjavfu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gwknmzwmu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gjyusnpwj.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/glxerlxoq.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gseybocqj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/glssfcvhk.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gqvvhzplr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvtcoun.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gpwacyzrn.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/glrjntjha.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/ggdjwbnvk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/grynylbzm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gbvwsbvam.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gpeeiwxxs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/ghkjwtuip.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gulsjpwoi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gcpaivlbd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gaoefvwrq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gsizmvjlm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gknajuyuq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gkyatukoc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gpyvmyfag.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gpphfgkfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/grjldibnk.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gckvuiwsp.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtpxsijek.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/guiujgolj.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/grryjdcme.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gtutjymee.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gqoflqyll.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gysqblwvx.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gfmyfbwxw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gtkpfylsk.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gbgommnnl.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/glwkpzgan.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gmhknbifu.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqmscemgp.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ghuhqkfcg.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gyerkcwxu.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gqkjoivfe.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gikxzdnzo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gteikccis.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gsjwazkmy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/glvgggwfw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gurqkydxo.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gffruvjta.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gibllnjcp.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/grxdtmfpl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gxfrffozk.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gwudcmqdc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gjqhczqgu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gjicsnraj.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/ggwdmddtz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gweqrfkua.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/ggzshugjd.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gxfnomzwk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gtvfqjtcm.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gleafnbjm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gikfqywfk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gigkdycjj.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gkbqaurjs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gwcalnxfo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gkdoyjcgf.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gkkqczyds.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/grmwovppb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/goxneagof.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gmzodyfii.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/grmxvrjgs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gdjepcwst.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gunwyycxt.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/geuinwvij.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkyneoeru.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gagaulgok.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ggaqqupdt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gmuhnghxy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gczuypdhc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gshckjtpd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/graqzwoak.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxgrguvzd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gbubiwuxb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gekggexwc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gpbejsojx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gwsnurutv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gelrgnape.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gutzkbokz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gweiiopqd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gorfttbmy.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcvwkxqyo.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gxmplszmg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gilkitwdt.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/guchvxqku.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/ggaamromi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gvultuktx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/grmbbgvva.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gyapiiuce.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gafuxcrer.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gheyejbwh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gltnvqlrr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfzcvyj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/goamqucdi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/geamjgums.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/ghdefysdl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ggyvkbwfz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/googemvhw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gdifjdtoe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gmylfxuls.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/guoyftfvj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gwekpwbzl.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gjcvextqb.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gryojzlch.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gaidnzgbq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gzgvugllx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gksavmsea.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gusjfuspr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtclecgnf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gywlnkeao.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gorgzrqkx.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gnipiuttb.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfatbbnkv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gefoeuxfo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgmieqat.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gftdiqhlc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gltnngdfa.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gkizhxaaj.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gqnowczeo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gbnvebhrs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gbzlsgkhi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gcuzxuief.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gzabmlubf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gaellhvlt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/ghnycgles.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gncvhkevf.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gudcheasi.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gnggvhwhx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gvozjsisi.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gtvzcnhes.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gofttkpop.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gkloluepw.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkssqfdxb.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gabdocmhy.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/glcunpmah.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gyiuchfrh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gjbwqrsqv.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnlkkqbfa.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gfdikkfrz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/goqzihtvx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gtjyrxnwz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gmxdondzo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/ghbcdhmss.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/ggeucdcrq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gytcbphug.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gctnxagdn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gikvrnoei.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gzzoesxmz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gplnfaelg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gvhrlikdt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gvwohnwwa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gjokxtdgf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gwoncexxc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gnunbswxe.sHtML


<!-- 参考信息 -->