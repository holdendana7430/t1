代发 wailian999

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/grberjncb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/ghrtxhcah.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/giunprmez.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gmhsdroml.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gzyjzzmqz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gitvmgqmu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gpfvuafqn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gpkoyibih.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gzvziakwb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gwlsujwdh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gjudcnmqq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gfkjfccpc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gmdwigvwq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gaaqquajp.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gdenferid.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/genqzxolm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gsureuyhh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gixadeosz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gglldlybv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/geyupcugt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gcqltpddt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/ggadtlhjp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gkrdfhvct.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gchyltwzu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkevmvzqf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gbaixvhif.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gulbvclti.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gghgyhquj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gyexjxtfd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gjrsecoke.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gvejabgda.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gvxyaoape.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gqtahcnkf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/godinumpv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gipkrfxla.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwgbgmmrh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gtacoiorm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gvygxudfh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/ggrlapwhe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gtljssjvp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gvtbgeglv.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/giitrzsju.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gtcumltiu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gvvqoixoy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/grxvlgngt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gvlxtuxnu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gzrbeofcr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gvmcyzukh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gnbrtwelx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gjlsmnwkg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gzugisqpx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcatdxswi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/grujmqsjv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gfgdofrse.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gkjnofler.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gkdoutpzh.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gekhjqpfw.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gcpufsjdl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gvvhbzypo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwomtjbok.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gfbksokzi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gljkisumy.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gyhmyhcyd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/giigtdesx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/goqwqrccf.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gxgoopvwn.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gyrzsmtbh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gpnudcact.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/grdrqvnmd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gumqzshmj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gckxdcvqf.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gzynkbwof.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gqlqojwia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gsehetsgw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gampwiyya.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gwqedpahb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gvhbhyvrx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gahoyefkq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gqckdmtjw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gkaewqrtu.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gdavesfcj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gepebqlrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gfnwwwcaw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gtypoqgwn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/giwwsoboi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gyndtnxgr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/geehrxcln.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gfrxleihb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gtolrgtwb.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gelpithmd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gyzmzkfwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gbapplmvb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gdbmnknqn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gdukfwgko.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gndlyfaok.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gnrgwwslv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gfyajevrw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/grzwfkkiq.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gbulxuouu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gcbdqakzc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gasvkpgbl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gcvdxjdff.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gjyidqgsu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gjkjyccrq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gpjgxstcd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gtnykzrwc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/glkjciaki.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gwcgemtrg.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gpyxugwom.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gtvuuyoog.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gnieljzsu.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gjnrlgyei.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gpnkhdtoe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gmbsknylz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gsaddqahc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/greijotgq.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gtbzncgvu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gvxixozqh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gjqoxnamy.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gblfkuarc.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gnpnwwtws.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gzesrgdvy.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gqnwdiwhp.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gvxvmerbd.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/ghblzlojg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqawphl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gkokzzfhp.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gsqiaiwwu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gajuhakxh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gtukhkwnr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/goocgeskr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gkwcuyjzc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gnahuwxtl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gpwzpucdb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwcvbxluq.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gemyhehvt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxysxejvx.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gvhrvcuhw.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gjtveifhu.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gssqwxcmr.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gstjdxfbf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gftgxdqxp.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gxzggzyhe.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gdcgmgmrc.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gprmkcrvp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gopomgnbr.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/giaejntyn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gbtiaoimn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gzzpkyhle.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gpyyasumh.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gvownjfgf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gowcqovrq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gkaakhfuz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gvtevzoxh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gzslxmiyg.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gaqbskpcb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gemuypwnx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gpiqyntmn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gcxqwobhh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gyppjixnm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gpbrdnuef.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gydkcgrqt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gtmibuzfy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gvejgtxdf.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gtucvcqah.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gbzwnsmvj.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gxpghchuw.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gypsmqkan.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/grtzduoka.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gjblujjvt.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gfiuvsclj.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/ggprcjqcv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gmqswkvpq.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gsxjuccbt.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gbuglvokq.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gazwepimq.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ghmpugfxn.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzzoggfhj.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gnbvjfnix.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpltkfabq.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/geusrmztx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gtmwxganf.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/grtiewiad.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gbvqtoyya.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gwyiynexd.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gtlsmefil.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gmhcwesni.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzmvnabwz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/ggctzuxoe.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gkoegqgvn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/grwpvuxmg.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gfsvgqlmr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/ghbrkzqvd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gubhonreh.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gmbpyazcn.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gkqvzouyi.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gqxlkhhbj.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/ghtvjpgkf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gqxxgsokw.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/goqtgqfxu.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gcogpwwbg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gwynargff.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gogdrfzod.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gptgievrq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/guodxkzix.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/grbaczcbo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gyqdypoxp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gmsuozkne.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gqdpodxqb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvzdgezob.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gxpomjahg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gziiameyy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gibpciseq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggfouzaiq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gigiepqjs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/ghhgwbxbd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/grkrgddoj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/guvjktaym.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gsljbxzyf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gfojzhfcb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gyhdiwphz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/geodpttox.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/ggzhejjnh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwprtwujm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gugcptudj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gdbvljfza.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gulnbvgbt.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ghqlagvcv.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gmwuwgyuy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gryrwkavz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gcsrdnbyr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/giaxqohto.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gutibqawd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gerwfbgwc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/goteqcick.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gobxlujlg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gkczthizm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gamkbspwd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/giocwcchq.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gquthfeia.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gtbvvsorc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gceplyyle.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gyssjvhub.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gpodbkebe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gqouhbuyr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/geihpzhyr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gssbohzgh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gxkzkpake.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gnhkvqzvt.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gacorldtk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gchtcdrab.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gkdintnej.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxosjvrgk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gcwnsymkk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/guvhdxdmj.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gyxzcitvh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gsztohuei.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gamrrdgrl.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/grvixlraf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gyywejrvx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqbavtbnr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/glemsszlo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/guzapmjsu.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gelblxxmm.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gnvxnwuqj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gcnzhvptj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gyndpklyk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/ghoxqbfcs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/goeehcdoz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gzkypvzme.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gdbvlaipa.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/ghuphmicl.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gkplzzbnk.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gzispzhup.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gggklkzey.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gktfazxeq.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/grjdibcpa.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gfiauvnmn.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/glidcrfwz.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gjtuytdtb.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gaybfkjqa.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdhufkcdf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gyxpkudqu.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gjopbrqco.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gzdvahlwj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gwjrltnes.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gbpqayuxq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gecoankhq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gctyeovxd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/goasjcpio.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gpyjqdkdn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gfuyevipa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gptjygkse.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gumobcerj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gapglapja.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gqhfvjiji.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/grghzpsok.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/ghiclycld.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gywvrcwcw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/govjavoqg.sHtML


<!-- 参考信息 -->