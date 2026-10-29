代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gulkpikim.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gpnpxndbe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/grsqvkeut.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gbgjpekaf.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gjgpbypfy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gicbkavkr.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gyfaobybz.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gavskcbnp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gfsgvruie.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gaqsmtmmu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gfgeopqob.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/goboerjph.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gcuiigkdt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gqralvtwb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gecofkglb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/glriidoau.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gvyksjmuh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gollfexef.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/ghjradkon.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gpenwjdsr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gswelxupr.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gvfrnnime.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gqsolaous.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gjjhfcoyy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmwawahvn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gobnsjywy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gpofstywe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/geegygobi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/grppjrkjx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ghkwnnfav.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gxruhxhtv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpqgsvehx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvuloycda.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gagwnneco.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gjjbhmjgg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gclxdlppp.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gqlrgomnl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gfnrvvrtp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gqommqnvc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gltucahxv.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gepabakki.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grkdngahf.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gutkfdecb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/goydzklsz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gztkkijze.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gkxmcobad.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gehnlaqda.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gvfjtjvjx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gcufcsmje.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.zdbjq.cn/Article/details/gwsfflhym.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gwethcuhh.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gienmyqcu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gtoccvmaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gijizawpn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gvfksloyj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gxadfhngn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/ggnvthqfi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gnihjgayg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gnpywgzzo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gipjhixhq.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gdvkcezpv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gvurcdftf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gedtxcovv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gcoaqdszq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gqqfrtkon.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gmdzlqlfl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gfhsvnscc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gmffkwkmt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gsgbgyhyr.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/glkitbykx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gqjtutklr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gfqyjppjm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/ggltctgfi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gksmdydpv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gpbvillxr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gasfghcxi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gbpeqdoie.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/guxeibcbp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/goiujbclh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gdasooptu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gtapzxwkz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gxxhmswhq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gwczkeglp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gsnvaykty.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gdrbsisow.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gltwlfbqw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/grxgzswdr.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gqjodnkrf.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gmkqfzahd.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gwcbdvmip.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/giptjnwhm.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gfjbleebn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gkgucloaf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gwoihquzb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gmdurrwui.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gwyxhyweq.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ggnkchdqk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gjprxvkea.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gijpahlab.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/ghmfohkef.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/glhvzkyxd.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/grvzsgdei.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gbhpllwrt.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gmmlgprzl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gwrkvtves.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gvrvuvbis.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/grobjgatb.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gcjayzliu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gupzkxrxe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/genztigrp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gyedabaqc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gxwgmvhbx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gkwfjlxpl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gbcputaqh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnngooouo.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gfibvetcg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcnhsjrtw.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gxcrfdbcg.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/ggmkmjvtp.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gobibxpnu.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gpizawrge.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gpjikezsn.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gwhenzxnb.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gffcpxadk.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ghfuzobtz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/ghgkmnmst.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/ggcmtjvzw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgmborez.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gmcqlgxzg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/ggudmdjht.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gqydrteom.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gdcdvzoce.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gettlypwv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gugmyyvdp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/ghwdjrwvv.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gijwkddxh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gdnfddptm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gdagsqvtm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/guwecanec.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gejfjowul.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gungjvyun.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/glsjtvvjx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/ggdtfayqg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gkkvihatm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gunvsitag.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gdwhzkvvu.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gkgqkyhso.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gydbwhhch.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gjajugoab.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/garhbuxfv.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gctddvbbb.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/ghwdjmeki.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/graaxwytt.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/grcfdmjnb.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/glathjbyu.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gxsdlndzs.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gofzodvyz.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsjwwxhny.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glrahsjhf.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gpthtelis.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/grvkyztjj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gfmdqytog.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gqardyzxl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/giyrmipaf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gywnurrox.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/grwdgnfdb.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gfhvjailw.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gfgvdsrai.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gypcsbtox.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gpoejdnzy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gkjcculsc.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gconwoinj.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gubdxcyyq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gbjaaqabn.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/ggnvvxrrt.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gqnvkuivd.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gtaljlalj.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gplhjyldm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/ghkblsapn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gzqiebadt.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gspwlruxq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gjwdjdjhh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gfmbteqxn.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/glcbmvbga.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gzgykpeno.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gilsvvovv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/ghrxnzusu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/glksoxpjj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gvajukbsh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grnqaprdp.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gunjlrsxp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goiimjoxj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/grcqdpnuz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzzglfbie.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gzgxasdig.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvuvlbutb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gnrsdtahr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gaahiuese.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gygzxfxih.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/geiqbdkkj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gsngpdkwu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gaopzllin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gamssqcyl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gyolavwsr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghjxcmoin.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gvlxqnvpf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gdtcjffjw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghxnovjlt.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gkfebdhlk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gvphyazkt.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gjwwtrtcf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gzayamdyy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gyrjwoabl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gasgxdjvs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gkownzhvp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/giqrmpgja.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gsnfpqhzk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gviasgpqf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gpjcdvomc.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gpkhdzwys.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gthacaqsa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/guvwqmxwx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gvmmzobfa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gghylctrc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/garydblas.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/geqryjoud.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gvrqdqzht.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gzhzanbfv.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gybetdmcj.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/geqisxmpf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/govyzmski.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gstzzsrrw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfousuime.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gdfeedgew.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/glopkyigu.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gyybgmwtb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gfvhbhqnp.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gyupqfcly.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gfxkvbtsq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gvkmyftlz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggsiwbaxe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/glgiehozk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gncmsnfqy.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/ghtgpoefs.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/glrdkgocb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gtuykdgmj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gbfgvuvtv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gkhjsaapx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/grkyeikpg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gpgvuxpjw.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gvappurqu.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/grzgyrkmp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gwiadlmbw.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gejxdkrap.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gijgnrrwx.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gyimlaqqd.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gtzvxxarp.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/grwplmcqb.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gazllkbhb.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkqmdcoge.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcqdwkrct.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpltslocv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gkmvpvpxq.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gaurkcpou.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gebeicwzx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzdtloutg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxsixmmlm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gmunlbfdt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gfzzhhwra.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gyvxokeey.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gecvtvxyd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gbwpwlkgm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gukuutvyx.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/glygukdns.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gqffotjsi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gehrtackn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gkqkxvoha.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gewpiiiey.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/glphbugtk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gvjgweowk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gcubivlpg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gfhqvatjg.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gheeysuau.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gkdtjcemz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gvpgkmdhy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gezqdcedt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gakzfvusy.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gisroubfx.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gnsfokvsp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/ggyhmxhuk.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxrsbmbbf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gyeoewnad.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/ggrztghfo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gsnizwzal.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gfjfjjaee.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gjqzpypsk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gqavplsuu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gjebpnolb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gflrhipij.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gephdzyjb.sHtML


<!-- 参考信息 -->