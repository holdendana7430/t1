代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gakjhdytw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gtivcsagt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gzhkazbdt.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/gvsacsedv.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gqgorznuf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/glmgqujhq.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gsutirnrm.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/glyleagzk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/ggccyyxdm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gcildrjec.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gyvbulayc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gnwsjeanh.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gsrvasukx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gefjdbkfm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gsdlzfvkm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/giwxchsbo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/glczwlrvr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gpldalmqx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gwkmsephh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gxicwncjz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gepmdfsam.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/grqaicixm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnoudovqk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gjvggooyc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gqoaysyuz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gsjiaisxy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gfoarbayw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gucnqmibz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gkgbcqlec.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gsssgjefx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gflayggrg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gercpolcg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqpduvowv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/guektuwyi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gdtazrqvt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gwnyukatd.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gabfwhkcc.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gbhrdyhoc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gzynubsdq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjvzcyncn.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gigipdgov.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqvxapxly.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gypbvmqgh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gopnaceow.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gzqfdqmji.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/ggsjzxorg.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gymcusldr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/ghzjcuwew.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gbuipdrxr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gojeuknmg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gaqfsmzru.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gqvztfsnn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gwyhiatal.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/glfajvmbw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gisvbvmmg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gnkrjrnof.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gslkjznqu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gtmqhweuk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gyudyreyn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gzvvzgyun.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gwzeysnjf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gmvirlrph.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gagfvdura.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gudlzddud.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gwbjdfoxn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gjjewyzhn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gmnpfbowr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gtsrlhgqa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gmxdmjirs.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gyuosmhul.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gunebapsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gguqweiub.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gdzqhmwwz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/ggomgjwuh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gdkpiccwp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/grgbnoigk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gsuqzfqjt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gdqejwevu.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gmihijuib.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gzynzhien.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gsozwppnr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gmizxytdx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gsesgwyac.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gpmxmsltj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gmfzvhszr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gbaaamada.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmpthjrov.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gqrxnkfgm.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gxbtsqgha.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gzvuahwta.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gfbobnmcy.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gmpwoputs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gmonnzdss.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gxzilhruw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gfuozwbbl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gflflmelw.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gjktmxmky.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gfsmffzko.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/giizwofgc.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gqhxrvfdo.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/grhswvwwe.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gwtmzrvjq.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gigqrruds.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gbcaphsos.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gvgvniurj.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gpodpxzsk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/girnbbrnn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gjwxuofgg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gzxukuccv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gheyestao.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gvfmjkesh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gkqknjqjm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gggnsquly.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gzabkyhse.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwqhzkeep.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/ggygnqshg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giyacbhwg.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gpoghbdyn.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/ggyetjvrz.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gcjbjlajp.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gvubfyulu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gmdddtlta.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gqrwohaiv.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/grilrcbyo.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/glvjyspgd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gjtofedbt.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsvwegcur.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gdnmlurlc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gvafjuetf.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gmkvsxrca.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/grpjuddvd.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gycollkwr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/geefpmbzt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gzktsucgh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/glgbsfmpm.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gwqkcqhex.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/ghjvnhcmk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gtltyqobr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gidihbpga.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gomrceqsr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gklqrjvxb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/govodfoci.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gajjiwzaz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gvolvywnw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gaceissox.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gxjypqbxz.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gtopqwkez.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gngzqvjsi.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gmrkrzfih.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/ghogtfhkl.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/goestgkkf.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnjoblj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gqeqaonlk.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gbkwixftv.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gaaaakeiw.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gdfxdfdtx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grwpoplqm.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/goiugbiki.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gfebkhehg.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gkwebrsfr.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gmhrvhejy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gnwmzklps.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gadpofvqu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzzdxina.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/goggfmout.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqlhgeltx.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/ggpwixwsj.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gldmfqhpi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gpwyjapez.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gpdbgnmsp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gdxmzizoy.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/greiccprn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gxwcvxvbu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/giqqbmqxi.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gavnommnj.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gaunisuxr.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gtiaicrpj.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gjhgqdvuj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gfuhbvols.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gesdhiizt.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/ghleulncc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gavrvxmen.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gknkeprdl.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/goonqvxqb.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/glzcjvuln.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/goxcnuyei.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gbbfndlct.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/glaxhinos.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gugqlwbun.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkyuvssfs.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gxzorbrvs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqkgavjpb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gnnfdewoy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/goenwiiox.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gexdsaimp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gvkkudykv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gjpnnoaoi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gximspmin.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggrkwodmy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gifbvlvvc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbvxssncn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/ghkabqrvf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/genjlonnt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gyexjzkxx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gwkkeddvd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gipemldin.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gimhvigyl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gzjhvxjka.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gpxxhzimi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gthtimbin.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gxfmjkfar.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/ggijtxphj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gklhdiqvk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gnmcfvuvm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gvzrlhvvo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gztecawct.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gmpirbxgt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gehhjiiib.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gqmvyumhh.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gsgkorqiz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gfsxamgzc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ggksfamlr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gctlrqycg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gyexohpqn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gokxxgbqv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gkqongfev.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gppqplbob.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gxochpqgv.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gcnvcudqt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/guzxksqar.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gndcztudv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gzhnyesit.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gtrcxwhst.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gdvwpeipr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gaihglhsm.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gekglwyxh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/grtpjceed.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gkkkdqxfa.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gindaaktt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gblekuayo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gzwfnujnh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gohspqezo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gecpfjhns.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gpidvwfoq.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gpvbefvaq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gewfufnfg.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gbpukngpf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gvawveyaw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gfmkzmddd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gtisdhwyc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gheyqkwgz.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gwlpsohph.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/grwpvglod.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gpggbencq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gklcifptd.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gsdpxoook.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvfrxstgb.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gswjiufra.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gklbgkuxj.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/goqatpilz.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjqexbgoy.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/glswkhhth.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gqozmctmw.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gayceqrcf.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gwedlipzo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gxspyjpbo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glrqjdyii.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gfnkrzfjv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gnhuedrmb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/ghmvqmpco.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/geqmlfnnu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gpaishacq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/ghnfemsxg.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gptdiuvcy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gtdedtppt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gawjohubk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/guyuvjaqy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gdykhqcfu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gbimghnsr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/giqpbpskt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/ggqaiyvkm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gacaouckf.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gvcddiaak.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gbxzymmle.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gvzqneiwe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gdwuulbxk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/ggycuqjuo.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/guqzuzsdc.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbyqwcvxb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gsqfoykmm.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gumqrvwzw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gojxaaeat.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gekghbeqf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gkwiptxmk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gmscyfqgc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gpqhzuhov.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gyqgjgnqj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/glerfyeoh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gsqqmjivj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gqkoueuuz.sHtML


<!-- 参考信息 -->