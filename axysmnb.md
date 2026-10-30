代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gnwhydoxb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gjdomcoyx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gnegpnvnh.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/glytybslz.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/gkxfrsszd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/grapqxqfz.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gheuahyev.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gzmslepva.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gljuzcvar.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gnqkzwlig.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/glzbimwzr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gnqftxmbn.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gkgffjbzq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gpinawdxq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gmhnzgoov.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gbwtxijui.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gbkxcujhi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gbdmtxtfc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gpvmivygp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gqacikmps.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gcelbhlrm.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gmwkintxf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gbkgkwefz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/geexofbjg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gitntpnxu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxxefdlzl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gyrammeot.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gpxaykqwm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/ggtllnwql.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gqbplyixk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gdhhniawy.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gjtthkzju.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gfpoecluu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gqwuyskjn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/ginsdsqmh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gqfqaaasf.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gwpsijoct.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gsjnkpwbo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/glksjuetv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzxxjhzhh.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gztkkebvk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjuywoqbo.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gczwlckbf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gbjnpymrb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gduwrveus.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gdhjgnzkc.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/guctfdpyz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gbyqrbldy.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gwapxhapi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gjzzqppem.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gdalqwozx.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gesfvxvuw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/guibhdzdi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gxukvkstw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/geowmuzwn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gjetwuvmp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gcvwoleyv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gzmyathha.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gpwpwlctx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gocmycndm.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gvfwxnsbi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/giowlyotl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gtnteawyl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gxmrwtlvs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gmpfrlqnv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gckvyxriy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gfgfzrpyb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gibravudh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gheqicgra.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gxibatgxf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gxkjwfriy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/glocndnhm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gjoczzhxn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gjbfgjrne.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/ggfdayjyj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/glsxxzwfk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gcampffjc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/grwlyetrj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gaszodlxo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/gqunlvvdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gillajxoj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gfexucxou.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gkkpvymdm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gdprurmfh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gkwzbeyvl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/ggyvzupnq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnoddupgg.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gvcmkqiwv.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/grvqxxbty.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/giohzuppf.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gmqfwajqy.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/ggsqcdbpa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/guecmonuu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gzblzssps.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gtjefvwkm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gfbhaaple.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gnbzqsuqr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/glwfzukvz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gbcswusce.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gdiaojsqf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gaclgsplu.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/ggesdfknx.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gyvjaugwl.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/ggtovffvw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/galxdiabh.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gxzpivxry.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gtccinwju.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gyffrzxrf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gusexafyd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gzqhwqtdw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/ggwjqpxwm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/grnnlfelx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gfnefpwqe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gskrmoyry.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvvrbwoeb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gciozxcqa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqplmgona.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gbmcahonv.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gcehywuzm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gfxcchoks.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyiifhoid.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvaiovrwm.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gdlpniuuu.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ggmrpuhvb.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/geamvbfzt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gqlnybhcd.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gxmxikpol.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/giskdnkww.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gcxauqava.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gomfqukea.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gznsgpuqo.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/ggimyqrds.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gghnomjyi.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gimslgbjc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/glvwvrxsm.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/greulkddy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gkgfmgkgb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gicnjnueb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ggkoksdaw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gwaptdwkc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gxohtcxcb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gputufcnu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gleptbziy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/ggefutcec.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gpqyhobaj.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/ghvdruqrg.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/ggndsmqzx.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gfpgrsrsl.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gcbfuziyc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gjjiaypsk.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gmstmseqw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gbxzmregx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gnqxwoyhx.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gdgikkzpv.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqirxyvem.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gjztopntf.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gtqcjyvqm.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyuexzuwh.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxbncuwoj.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gcdtutvdj.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gexopokhy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gvoeolxrh.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gzuiawmon.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gbxszgphm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gxctmlhkf.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gvpsulbmg.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gdlflmjgb.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gwbkcgryk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gxlzldbad.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/godmbezbd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gupbjgixv.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gidufmabk.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gspcfyiih.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gkkkwpenw.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gpelbmqjs.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gcnvcddwt.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gngocamvd.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/ggzqzezwr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gxdxbsqzk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gfvmtruvh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gaiqwqigp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gawsgxqfa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gcgnpyrvr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gsifwmgeh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gnwpkvwkl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gvcmbxeoo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gkwpwxjnr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/grgggyqsr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gvjfeyeqr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqkzbqoux.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gdxkfaxtz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfkenbmco.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gjtiybnwj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/glurmqhwg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gnnhvmrfa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjbzyyrcl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gbeqojyrk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnqsoresx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glsdfkrar.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gtqpserct.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtmipnqyv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gjyonsmaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gswvqbymr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gbzvugkjt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/giawjffqe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gerifarvq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gxwobenei.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gkkzzaxrj.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gsrotlicm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gehqxdpau.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gdjisdmsq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gezourfxv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gewxmrcos.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gxxklqokt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ggmiuvulr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gpmkhbzez.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gtixefvln.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gsgqmnnvu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gzsydxweg.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gomldllfe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gwpwkrxby.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/glbzaugyf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grgvtyjxt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gzljbjnpg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gshpquoxx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/grywlaejt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmlwnzyy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gygdhgsft.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gclchksdz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gfttjutns.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gtmckfiwj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gnitabhye.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvtudbwgo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gxtkyevqw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gaxfgsvep.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gvlarybtg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gwjplhnve.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gxwkvaooz.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/guthnrjzu.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gqvjoyrhl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gdpbjitsm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqdwebwvv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gfwjmdjiz.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gozbjqnon.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gbonmhbrk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gmuztryfz.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/goyagzlnv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gsspprbej.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gxavdvsou.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gjrvvgxni.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwfthvn.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gjwfsjwys.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gccutjdiu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gqueauhoi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gikpcvluc.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gtqvvzwks.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gzisishek.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gihgifmzf.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqgrdsbxi.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpgldpktv.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gbraulxyu.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gwkekmazy.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/ggmhchroj.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glicrgveh.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gsdddshzj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/glsaempnb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gcudkemqc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gxjzsrhqk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gdassuqzr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gomuivvwk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gfsuumrbn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvfccpnbg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gibxxsyop.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gqickuthl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gowcomfqh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gkrrnjood.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/grxdlqftx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gzbdjuvyt.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gzefdvqus.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/ggyzjzedy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gjcqgaxkk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gefhuhcmg.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gnelnepds.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/grpwllxem.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/ghtkauqyz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gqrztopwq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gvmwnobvi.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gvdjzlmfg.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsueqkhyq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gjmdrgcmc.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggdweuzoh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gncjkolvp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gixpauagq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gvdqcqbin.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gpwbgjgob.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gpwmfbifv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/geomrtscf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/ggetmhptc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gvgapsald.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gtuowrfev.sHtML


<!-- 参考信息 -->