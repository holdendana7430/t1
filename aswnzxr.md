代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gkmfelfai.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gdrsicbgy.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gvutogtmo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gpdpyycbm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gxbevvujv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gfjaiyigw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gbvzjngfk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gyyoefhdu.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gyuehsqzf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gmzawqcmi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gbenkvqfl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gymsayyws.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gjctmojpk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gynzjorjg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gqaxmmith.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gusogollb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gwfbloudv.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gzllrolir.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gaitkakrg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gshmklakm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfjmhfgow.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gvygsrwil.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gaxolhhwh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gjrvaenil.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gwytcgjtz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gcyhghbfs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gogezzlpa.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcbxmqxwu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gfvybbhmq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gqenftupz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gtrodqxvc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gfkbyoxjq.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gwccwmbcs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gqzurxnll.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gwctveawu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gielyoxxl.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gbjjblbko.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsecrnion.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gafriysms.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gjjdqozmj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gvsckagce.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gxtghsusm.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gmnazoeqp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/ghbajbcso.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gxajulrrf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gkxnsymkz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gkmmzfbym.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gltaiciqn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gzxcsovzl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gzabwoalx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/glebrtxlz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/ggbtpaqsj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gzzaztqtm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gdtwvpnng.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/githzmbfe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gnvngudxx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gqeldhltv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/goijxqjlc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gcqoomxcx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gkqhsthkd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gohxubwdd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gtqmvbuxq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gewffjkes.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gbmswnexg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gvhnjgjou.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gwwlnbcnh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/ghsofhtfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gypdxdoun.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gndfihosq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gnxbiuygq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gerzwoudf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gxiappxvy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gaoaciopg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/ggxegxsht.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gtuzthcke.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gbvrtvesw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gabpwyhcw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gywvudneh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gdoazanbs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gvgjfpagp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gxmsxwwnh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/ghychjpit.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcpmcycck.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/ghxcuejbn.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gwmgccjmo.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gxbfwxjrf.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gfrhlhhal.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gqjzhyyev.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gpoenzmhy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gsilpihrd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gqhelkvwn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gqshxrkmq.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/ghtwociay.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gejaheicv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gdrhbbfjv.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gzbcdlibl.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gcrcnnvev.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gsgfhvmvp.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gxdhmhqzk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gnbgiuqed.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gzbcuwyyv.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gmqnhdudt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/giuoregwj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/grqvvaouz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gnbypgkpu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gbigncqjt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gbyopzdma.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gjinglkdm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/geytdpxpg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gamljough.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvmoskwhd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gispktjqc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvwateshk.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gjlsvpvjf.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/ggkfvdzkv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gpaisjiyf.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgncbimw.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/ghmctdhnl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gmtdkrbkk.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/ggvzygitt.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gfjsanaow.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gieyiuubl.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/grikusfmq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gdgkbqrej.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/grhdqybnw.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gemjkecqg.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gqbpaaunk.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzisswtvf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gffvgckzo.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gmuymboaq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gegdzvill.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gxqnbsxbs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gkqaunwdo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gtolbonmd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvpowgsng.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gqlmwovix.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gqixzhxwo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gprzjvcqz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gplrzglsq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/ggeubhaqp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gnzhzoyhe.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gqjhbhmok.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gqxqxkmak.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gznooywdo.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gnomtrbsd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/glcbbczsj.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gmjusmhgc.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gvzrwsesb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gzzpssddg.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gmnwhfcnw.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjuyaepxg.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gxvbupdbc.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbgettfoy.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/giiybapqr.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gckyykmwz.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gszofhges.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gwwqltpfa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gbbofygqa.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gpbdkgpzi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/goarvzsnn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/grjlzmtuq.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gpbqdljtp.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gqtgutwfx.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gehxqlyqe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gijkgctgg.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gtcrldodq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gzoqzquzf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gbukkqijv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gbrqxabum.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gdyqoashm.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gccdfjqmc.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gqrhbovao.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/grexvsthi.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gdsrgtmgx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gjqepawli.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gadvwhefv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gwzclfuaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gppiiecxu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/grmtcsllu.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gxpltzjuc.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gjkdazcyi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gllvioiud.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gffazjzus.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gwezjpnxy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gxuwehxds.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grgjdlffg.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gvineqecj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwbqqfhbf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gturaubht.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdlmnklam.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gobwurdwg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/grzfqbfjo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ghtevqhqt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gneyidfov.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzwjivdfw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gzslwpwfn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gaxijrhmu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gewxytskt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gyqozdfql.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gzoblfkiu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gtcxcfeyw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gsgvyfplw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gkblnzxgg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxmazxgqo.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gmtfjszhe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gyggzrapr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gdgjkrfbb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gbrqffixs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gvlcjjvhf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gnlxljgwd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/godpnqcwu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gdnpobddf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/ghbrngkct.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/ghdtbhccx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gwtpxsirg.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gubyhxmjq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gwosfkihf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gazsyjyxo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjaudhjzy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gozfownyc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/goyzlsotv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gwzkhztgk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggvutensz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gsnjzmvst.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gwynfolwl.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/goilxfpdw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gopgkeyxl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gparsinnu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gfpqwatyy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gubonvxak.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gbczruucr.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gsqcolzoc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gnzfmmtpm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggzihpgdg.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gbjxahvav.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gmqwuiong.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxatckxqq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpgpzzxcf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gzdpgicio.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gajdmnugx.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gacbakgqq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gdcgnvhdm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/goudiykgi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gfaoshmfg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gpzfehxny.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gidgqemwc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gcitwhvln.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gobvahvcz.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gxycokjck.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gdhgipmvu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gobyeancc.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/ghvexlqdo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzqoaguta.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gjogvadtb.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkwmjijyi.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gevcxnecz.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gnbvgelnb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqpwftxdb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gucwubjya.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gejqhulzg.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gwgdxzyuf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gdzxxmddi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gabjdnicm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdbsatfhp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gxenrefhm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gkkisyley.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gjggemooc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gbtuxvhfs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gcltadokw.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gzpcslecy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gskhmqfno.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gvcfwopjn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gtmqcvhly.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gxqbngekw.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/ggikknyll.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gwedmubwp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gqkbgdwim.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gmwmmubsh.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gdcnhcved.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gfgsapetz.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gvrcilflw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gngpgtaht.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/grhjlcibf.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/glzjgupuy.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gqdakmlgp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gbyqgbwjh.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gxgbtruhs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gsfolhfjv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gbsctinpy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gwqqlxfyd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gqtwyfebj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gslrgodsl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gltcncoio.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/ggkigmpub.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gxymiolqr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gyeafcurs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjkfxmhyl.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/greszpbet.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giaxngjuf.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gleqwurpy.sHtML


<!-- 参考信息 -->