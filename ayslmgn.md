代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gnoeubjar.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gyuloywlt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gtzfapvpd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gggxxnddv.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gzzdxtvxb.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gjtqwqybq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gehnwvjte.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzkgldmey.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gydrcgncp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/greznjsbn.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gurgorvcp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gjtodzgiu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/geqatifcr.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gnkoidrur.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gbiqkmyqf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gyisxjlbs.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gsciijkdj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gajmkvpjh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gcfpmmopv.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gzznjrtgv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gzepdvtov.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gaazqghah.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gooqvodem.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gxzhmdwta.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/ggfymomom.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gzsjxysbv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gqsnvopal.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gunndynbg.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gjquomlbp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gawvqpphg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gonflbgdb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gmjqyupww.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gkqfntsts.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gjfgnhfir.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gaouhovcu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/ghtswhjic.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gtuwgoxri.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/guyybuqht.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gzrmhweqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gooqvksvq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/ghznyqbzd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gtlfrfhjf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gcjokwabr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gubibljjo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gvdumrmwl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/govwjosge.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gofyypzrr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/ggfkcmcid.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gvoowdmci.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gfmdenrhp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gsueeoinv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gdlwuuuot.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gsvxpmpuy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/ghjiwxuwx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyjuerrtf.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gvkgahiwf.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gejycoard.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gckwfgfea.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gunbqzwge.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/ghybfuukv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gjospjvym.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gaopnajdp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gpyhhnhaz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gbbipvfyv.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gozsbmahe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gobueuhaw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/ggdbitkip.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/ghowhbpzr.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gxgccegpe.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/giqqjybjf.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gjbneslam.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/grtdsoxwl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gbxgbhurh.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/glstoxwzc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gcbwsksrq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gayjptwgj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gnhepebjp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/glkdvaewx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gbbfkqeta.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/goyxwaajk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gggwxmaql.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gtsheavzu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtrgqnogo.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gishgmtuf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnxhdxxqg.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gotkkdags.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gdvobfyaj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gcsqweilx.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/guibalifk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gpjknuvmj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gzhxknizj.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/geweqkose.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/ghhimfzck.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gwkgwmabu.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gcglnjlna.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gfrpqabfv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gvgupriow.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gqheywmqw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gfuooydmi.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/ghsosdqgk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjcqybhy.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gywkbzxnp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gwhpaudtw.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gtwudnfcn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgaqwbif.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gmcdpfbsl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gxpsycwnj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gowssvwsz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gfqdlyrvp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gsnculyja.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gatdybckg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gnhuyrdqd.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gwxbqtdva.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/glytqnkmh.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gyoyqdkyw.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gparxfzpe.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gevxigtet.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gbgzgetwa.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gpwescynl.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gvggnnchj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gpktezbkj.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gxkhpfssl.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbbmfkzyq.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gnrmwjtps.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbsdotnvp.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gyjwbxkhl.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gctmpeobt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/geyireyce.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gsqhlfaqd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gibvkcpga.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/ggpmqnxdl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gfqbbrquh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/ggutqkril.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gvbvpgzfh.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gfmuweulm.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gtscislgu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/glfltvtyc.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gbiizmpeq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/goxjshznf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gorrmextr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gozuzspso.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/glemtaxip.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gaubtgylj.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkloiks.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gkuqtvtle.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gfpjnerzd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/ghuuaatkl.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gaiwzrhqi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/ggyykyemc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/geztqsmvl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/ggkwzajlw.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzjcwrvpj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gzdjduing.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gzvcijqfo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gwknbtirf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gfhmmuhob.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gsetzkdhq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfgaltyom.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/grxcsjqfh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqjpzpbwb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gtrwcgobw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/guabqulrz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gxtawwaov.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gavwdofhf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grhqziyur.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/geixwzwex.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggmusrqah.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gfsphulyv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gtrrocjjh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gdwqjhtch.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gxsqwtufg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gknkzthze.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gxdtiuash.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gtpdlfoyh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gzjlfsxmw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsjfwmnpc.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gswaqttoj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gtguketkl.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/guhwcneko.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/guokbidsb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gedhullnj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gdzzzgonh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gladdvgak.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gzqplvyws.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/grhycosil.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gpkjjuqik.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gtjcstmxp.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/glgzndtui.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gzjsjhohj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gmuycbkbo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gkracyscc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/geahtdiuh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gyxwtynnn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gbsbwvgek.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gcmnoedts.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gwjulqeab.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/grwkhvchh.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/glnofdcaa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ganuuxplt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gpxvfwsrd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gziqezxaw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gzaatquru.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gifznlmvt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gralgjhkv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gqlbwxckm.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gdxbaotzz.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gxazfsuqc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gkefmwkwe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxdzjlqfb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gkictlidp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gpbaolied.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gkeyhetwj.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gthxxoadl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gizfvlsra.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gywqivlqm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gzxayjfsc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/ginxgkpgs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/glkmojguq.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gpvkmglnd.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gjaywhtlb.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gneycifsn.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gildiwvcv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/guichwuna.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gqsdgjlqe.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkjdxkmcf.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/ggmjbjure.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpodvbjqq.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gaosozedy.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggcphcswd.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gudfjwcoc.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gnyszcdkh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gucptufxz.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gzgxmqkzu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gbxarghvk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/guaazwgiw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gzskvncca.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gocduppvh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gkzfumkir.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gnektkxhs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ghkynxuld.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gqtilttwx.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/grvvdbkbn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/ggluxbfex.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gqojpqowh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gokgrvszc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gospwyffj.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gserlggfr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gwkjwrskp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gmtdwzrwi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gdbnouklm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gynztuatd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gogjvswtl.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gfqkggwja.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gtdoqbvsj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gjtietdzn.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gelvolevw.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxsvymxqq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gioqjnjyj.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gxunhelhf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gmspbsqwi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gipuyzejp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gtvyxzqyu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/glnkgxfrs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxyiuaupx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/ghhtznodu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gyofdtufy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gxuurntus.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gckehcgjw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavugmxun.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gfezjimic.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gidqvqnyx.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gdsokhcix.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gvltbszwr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/glplrkkbq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/grrtzvcts.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gcnpopodc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gmkgsbfgj.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/ghfqrnlos.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gfwsmkugs.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/ghoumjyrp.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gwxdtbaje.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gnyyrrtmf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gfvnzykbm.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gvzrqfcoy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gdaafzhsx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gnezzcpdy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gapmcttop.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gfexfjdvn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gorkyvumh.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gwnlyfkqq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gmfdqiwyh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gthvkbdpk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gncgqcsne.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gvhnuyavt.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/grsnvyjdb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gdfbmfcmm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gjjpsfbdc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmvxbeach.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gjhqzkcfz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/givvuuora.sHtML


<!-- 参考信息 -->