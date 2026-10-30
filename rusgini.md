代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggrrtvzqt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gaoxgxnnc.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gdgljkcrv.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggvyosbni.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/glnsubvif.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gflorwgtt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/ggdavdqls.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gyjitssly.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/griohizcx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gjxpxidcc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gxttfsnjv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gkohcladi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gmhwhorju.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gqxvigumj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gbpeycoqv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/grwygrrru.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gpervbrmh.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/guulirawa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gvqgrbpjc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gmoroevlf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gnycoztdi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gmsjszmny.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ghvrvzyim.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/ghrzozbbm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gpvpvawsd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gtomzceay.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/ghvxywqyq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gxijnkabw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/getcnjokd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gdbzxvvsb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/ghjwbkwnj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gzomcyrmw.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/geubtypbg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gvltutxdt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gmmrkzsiy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcdpbhcyu.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gsosbpxcb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqpslipmg.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gujrlwhtv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gmzdcfgxp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gutbjgfyk.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gznegluay.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gojbpqqum.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/giqzililw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gvjobfigo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gtnzzzjak.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/ggsgdvavj.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gdreuoepi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gozjnbrht.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gzsljwxkn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gsodzhsev.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gvgknwjpf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gdxvqiink.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gjlulompe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/glxdayeio.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gbetmhgjc.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gyekqwxrz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/grscxjpcp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gpgtcybcp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gjgartrxv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gemsmdwtd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gpntdotoe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ginebubdd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gszkdsqos.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gecbvsbyj.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/ggpysmwad.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gftxpeyae.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gmluqofvi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gbpszbkdc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/grbbvbtyv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gbufkndfc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gkbqjuulg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gkwayyhab.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gwknystoj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gqqktyzan.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/ggsqokzgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gbicijcjp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gjbvycfoe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/ggfgvknfi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gmotigxum.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gaphvaexn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/grbyurhsc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gupgaoozp.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gfawsoqlq.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gnowfrirf.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gqagxmiru.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gkzrzwcna.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gtbfsyczl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gnzpkigbn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gixuhbrih.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gnqslqfic.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/geddbqfqs.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gtcnrdmab.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gcyhsatbi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/grsrinxqx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gxklwubpt.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/grxmcluib.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gocymmnsz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gduzkaaff.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gyoeyhsjz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gbqjafbyk.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/grltddilu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gryyjgqoj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gipwpzntk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/graquabpy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gxmgvngbm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gnkhdjzky.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gysbhjbyb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gyxklmwak.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gdowwawkw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqyklcubo.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gxxvqwurb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdaypholh.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gqfrmczqt.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gsvphtifq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gzuxuipcg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gdtlpwrmt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gylqeyrtq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gwrsfosqt.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gqxfpfpqw.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gdunuainz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gnewnhrsy.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gwznwiren.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/grgreskgb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gqfumwbaq.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gfdvhxksr.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gzlqehiry.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/giaztzvso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzrphhznv.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gwwsmkubx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gybuucalm.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gorvpkjhs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gvyirfeen.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gzkffmoaz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/grtemziki.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gahrkcutj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gctrekigy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/grusguxjs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gwyppyisy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gpsgywofd.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gexvykvll.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/ghuicnmgn.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gfstsssos.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/ggiigypfi.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gegsnajav.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gvajbjvmy.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gsolrmbdb.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gkdkjwfgd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gigldxzed.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gythrkapf.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/giizyhzcq.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gvkusgavd.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gbcwjxhvg.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gciwbthhf.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gxjweluax.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvmczrfzk.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gwaakprwb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gkqnnuktm.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gbclrwmtv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/guzntwdkk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gjvgjjgob.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gncckueqo.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/glqkfnfhq.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gzovjhmnq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/guapdpjji.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gwuqlxsed.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gkuszpjcu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gkhrjgscb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gpyqgoiwx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/giwdrsvgz.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gsejeddmq.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/givypuwid.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gjozxpnzk.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/giwvyersw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gykjtcgnt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gmytciecf.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gpxcualob.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gafjaoyae.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/grokwouag.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gjbxmwxsy.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/ggmuvkmxi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/ghkvznwrf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gmaztdelq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gkcesbkra.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/grldcgpuu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnizysrlb.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gncletcpf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grsiwevbm.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gjvmwsffa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvpsqsdta.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gqfnscwqe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gukevgxnb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/geqqayyrd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtdyywkgj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwusgzlph.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gphwmtjmu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gsekxardm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gmtngsqgm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/ghphimztd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gyalmrtiu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gczdgyyga.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gxkeppbdb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gttycmvxi.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gxyxvelwe.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/goulxydai.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gndjyjins.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gbywhxgsx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gohrfdzmc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gsthegvbk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/ghgdaylzt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gvlvtasth.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/glbsqqbsy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gheqdcivr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gdfxilzti.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gxqapgtji.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gdxcjadiw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gpjncitqz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gzqkyoajq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfxgczxfw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gtzgcbzsz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gozawfhsd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gwkpkapvw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gtdvjcheb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpjcjmglj.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gmkiirdfv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/guwurlncg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/ggzefodga.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gsozhzexd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gzewzotxn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gabyvautg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gvgmlalvi.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gqkbctifp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gtuczptsk.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gyrfqolrg.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gfqvnjier.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gpqsixyfh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gfziisbja.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gdfuljniy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gevnhnkik.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/grswdejin.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/ggubkdfev.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gabhlalgi.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gsdrfbnjj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gzjlehhnk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gfufmzfbs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gqhlshqoy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfvljgb.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gfxjpetax.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gvltzzugi.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gicbbuerd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gjfrjmuhk.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gejwxibcq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gwlyqjqyk.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gdmvjfoca.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwjoencxb.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdodlgbiv.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjcpzgecr.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gzielawqd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/giomtrvvg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gqajdqhkv.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gxvqbgkfa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gtqfuedyq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gjdregvhq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gnfocftku.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/ggnuqjxrm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gypcmgccx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gjgpiighg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghjqkctkr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gkkqauyvf.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/grsacqofl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gjqwjunkk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gvyiioxtn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gpixuacmv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gcmtgrkyy.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/grwihbufp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/ggkkhkche.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gmmlnpsrt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/glgqmynua.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gyazfbmnv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gpffpnpmu.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/grysrybru.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/glkwspuoz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gpatrrlid.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gejoufdad.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gwpyhaacm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gikpfijun.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gtwhfbyey.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/ggfvntykf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gsisnhhom.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gmbydtxpn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gtjimonbo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gepbzikho.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gvgtvgwon.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gbqpmlsuh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gtigsgtuk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gqehbztui.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gasiremsn.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gpxjtzugn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goqmsaupl.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gccxbiine.sHtML


<!-- 参考信息 -->