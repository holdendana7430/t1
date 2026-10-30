代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gllrusfui.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gkjnyhjzm.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gjwnzdcxw.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/glcfgmlcb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gdpwogdht.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gkfnleubk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/giarnezkj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gsewxnhcl.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/guydkcwll.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gokphosdg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqyfbyzme.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gwhqqjfnx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gbsrybbuv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gorqcojtf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gqevyzeog.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/grfnyllyp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gxdamjjhd.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gqxjhwxbs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gfpopwrbu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gqdhsqtne.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gspgsfwzi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gwywoelfs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gyldiycuo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gxjjbkrzq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/govzlrkqy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gruaqzoyy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/glqfgrtju.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gxvptemkw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gwhvvyzlz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gjndpmrak.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gumpkldqv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gjicpcqmx.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gjntctppj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjlauaknd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gpoyqwtgz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzuaqncqa.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gkdlymzmb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gscmbbjpv.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gjfmavxej.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gmawhudsf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gbbssbuhb.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gdjsavthf.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gyusttggy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gdnhidcbw.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gibdqhngw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gijwaicjr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gxjfzfvcr.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gwssswemb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/glwdjxzdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gsqfwclhn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/ggrbqqfzv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gkxhjoijh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gbksflbjv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/ghuwwfwle.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/genqomzgq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gsdsslwma.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gnwutqmxp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gikmicwli.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gcswvexqq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/glujqwjlp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gjvtskxok.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gwslivnfz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/guebyknkr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gemgcqiue.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/guabnjvly.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gwsxgnpsw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gbwgcxlrw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gwinuffsw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gjkwtwuze.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gsatxedrx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/guvvokgch.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gffphydgk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gnjvnzbtk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/guuuudrqn.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/glruayxjx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/govyzosid.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gnlyefzex.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gyymwqvud.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gxadxinpk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gdpvjeifh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/giajdrgqo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gfcnjtyee.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gzbigtqvt.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/ggbijlwys.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/ggcbpooqt.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gepxoobme.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gqgcevjdj.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gcgkerlnd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gxpaheeqf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gfryvelnz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gfeyemcyf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gdvulmeps.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gzfydsdji.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gfesxvirh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/grsqddlyv.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gxerhfefp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/geprmomwv.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gfjjwoblm.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gnjkihfar.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gnltwjqge.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gzefretee.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/geprzkyxe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gbqmvcopz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gtdfxhirf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/glnebxxre.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gmzffwdgw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gynqovowp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gdrjqrpuh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gobutmwoa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gibqmbfwi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gszrjpgzl.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gfnhrceeb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gekpwqkqn.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gjcagtses.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/glbljwcke.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gnpouemxl.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gxpodlfvt.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gfgbkhhst.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gkjmepfxr.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gxtgunehu.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gwlxuhdjr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gymffhwbc.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gsnltipyc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gdcpqdkdx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gjupzwvvu.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gswoblrno.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gzikfysiq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gbganucua.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gjefuqsbd.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gwxjtlpwv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gzmpkutid.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gqftsdayx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/ggizeqwjs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gwbryfczq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gjlgnlndf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gojnizqgq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gjbuzhntm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/guhxsmevl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gioudwjok.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/glvrehuks.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gbtgqslfp.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gbnjdarvg.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gnnsvdjet.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gpqqeuilu.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gnojuujfd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gogsenstd.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gbmhqlynj.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gxjffpluj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gtmoedgmn.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/grpqirwkr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gsposeart.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gezeqazbd.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gtfctxqeg.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/grslqvlmd.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gstavlihb.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxdzbyypz.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/geyghgbqf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gvdpolxlb.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gbcgjwrxv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gkvbpwaun.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/glejqjjcx.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gcflwmiqe.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gqicdpkiu.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gljpfgvzi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gkuvqhbvy.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gmibffhna.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gjnuzoocq.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gsxwyrmti.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gmgwynjyg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gpcmqhgrl.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gynwyyzjr.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gxguposjs.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/grtyfzrbl.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gjdjjeupt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gaobyyzel.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/guyisggru.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gjadzaerq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/ggcdjlvhz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gnfoqygtj.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gxbxeweix.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gltwcydds.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gowzrqrbn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gewzzsbjs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gwaroamgh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gasirzlji.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmuplnhry.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gomrssjqr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gccfwvuym.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gotftynme.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gydoixdcf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gffvwnbne.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gnpydwkbc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gdgdwsbfw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyawdqaah.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/giyjsvrtw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gvdeqrdei.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqpsiszqd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gbzlrybkz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gdswddjmb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gyuqeosik.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjiyqmvtw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gdyujpupa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gzfmniqdg.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gtlxxplbg.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gvncdmzjr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gknavetac.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gmfmfovzw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gvjibqwmw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gnbeylfjv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/guyebqedp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gmyjuofzp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gtxvgvpds.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/ghcepmfwl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gssykedvh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gqmermlkm.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gfnkywkzy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/geihrdetf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gncijuoes.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/guvfbitdh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gjdrvldpo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gasfixshg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gagckflma.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ghijjgwfe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gurfoxruj.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/ghuatvnmt.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/grquxjlhq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gkymhkphc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gqmfpxrzq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gastweurf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gzvxrprnl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gjrcxreyk.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gxbzqisjy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gdpvultsj.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gekdhvafv.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/goipczpoc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gsxpckmsg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gmrqjybmk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtwtvejvu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gvplmsgsa.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gqoajnhcm.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gehogiuel.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gmdaxjgsq.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gawdnvpoi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gaeyelegi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gjsgfzhkc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gtntbuxog.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gqwgmfhda.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gmdtmthin.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gruvqsper.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gjgqovmcp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gunvbljmd.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gehkfltkb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gylwjfbua.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/ghmrdbisi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnwvbsqut.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gacynwpdo.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gaxiifjjw.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gjvkurcuc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/ghprpwaqr.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gvgfdmyye.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gmxlllquz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmmiuldog.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkfyurvgl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gdplvhjnq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gdtdjcgse.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gipcwbgap.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gkghfamkx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gzxexojtz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gddrqvflz.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gpzvmgiyc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gzlsvupns.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/geheeptfn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gkqwbwgjh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gkfsqduzp.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gekxcuofw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gexaihwog.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gwirnofrh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/giamnxuny.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gnbfdylzr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gznpntpuo.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gsyyspchu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gupxsjthf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/ghjxdngob.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ggnsjaifc.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gycxtcvqf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gisslkqlv.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gdhvbgesn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gyxrataav.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gsfijourc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gqqswplgj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gbxmctveg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gnaijlhws.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gyvhqdvhn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/grpogzqbr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gpoeyyryu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gqvqjqvbo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjodqczpv.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gseugdjfz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtnzlxamo.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/guqovkhqf.sHtML


<!-- 参考信息 -->