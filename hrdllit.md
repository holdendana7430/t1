代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/grdvkwzgh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/grxjziaxh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gxcccyhkz.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gufylfcam.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gmluvdeic.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gtfwaaaea.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gcvefdmyi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gvwgdkhhy.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gtklbeygb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gczsspsjo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/grqnybkxo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grdpfgwap.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gscithenz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzfzmlgqe.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gicyontgt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/ghyrezsvx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gysxapsrh.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gdhpocvha.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gkayupqfr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/glwlffdfk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/girrftulc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/ghqobocuo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/ghvpeezzc.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gjygftmgh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/ggvthlidi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gotjryzhf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gtpyuyrqx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gskucimac.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gogqllfuj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gfcrmbsed.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gpbmwrjvr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gkdrpojrk.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gfuqybsfm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/ggyqortes.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gdzibgdes.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gwexsuozx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gysxwdbil.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gelvucrbg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gqmjobwfj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gdyqyhudm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gcfprqorh.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gzujorgrd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gpaueftbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gmgxrxsuj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gwzdoegmo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gwpxdulic.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gpipasxlv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gkwpejmpi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gydzfobjb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gaspdwrlv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gqlrbnjut.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/ggllicpzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gnsquprqr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gukcwhxgh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gfvaieyuh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/geayxepca.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gaikvpepn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gfzecwodj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxqfulzty.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gjbweagid.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/glzmdocht.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gmfrzroos.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gpbuafziy.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gxtzfudco.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjhlmekv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gpuqtuwpm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gsmolujps.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gfttxhjzz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gzeiypjce.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gbpolkjbe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/grovqalcd.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gurcrjfcw.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gcwhkilhg.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/glfulzfak.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gvbkknllu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gzlslclqg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/guudqgwou.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/glnsnjdtc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/guaodreop.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gzvuntcec.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gzmujsmlf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gcypknpnm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gorjvygfu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gvzlwfiia.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gsggkcczt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/ghuudowew.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggdrxytlq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/ghgovqqhp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grsfmcquo.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/glvlvfiqr.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gocknihhz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/goyetzccz.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gjvpvemjd.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gredzeteg.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ghkxhvcja.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gcsbxkgsc.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gjuszhyyv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/goboksgfi.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gjsojdrep.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gajtwrmqh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/glpgysoig.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gyyhkdtze.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/ggyyuizwp.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gtjkfitnu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gzcjzsjqg.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/glcdnwhyb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/golrbtfdj.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gaeyvhgzv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gonhvpcmi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gtwwcbwpn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gkotkiwcy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gsjrfjagy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gyqgrtwxz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gwdjtjint.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gcvqapgqo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gzxuxcnvb.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gqextmvmt.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gupbxxnww.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gujcqiczl.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/ghgwpugmc.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gcnpvvxzl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gltzptsro.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/getxdbaos.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gtrsfusar.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/glqacebqu.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gfekzyiem.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtngmnmfh.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/glpynigfs.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/grnnjnnag.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpzjmaabe.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gvydakxxs.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gfjqshgsl.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gsslcxvpk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gksneutdu.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gzprdclxj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gzmrdupfb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/geqpvlsbk.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gzsbisjkp.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gbbocnzzr.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gcadbfeqy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gmqmhxajo.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gaavrqfhc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gjumfjptf.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gxutwwylj.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gtuaskggt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gbuygvcky.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/glcrwmqcb.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gulzekhnl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gogwwelwi.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gtjhhtrii.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gnumrrlkd.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gdxxwanbl.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gxejkbllj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/giixmhjti.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gqhhoxwvz.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gcaousnyu.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gnzadtjvo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gwshawpgb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gqtndgtcg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/geojgzibx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gxsjqtjhn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gshbrfztz.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/ggizqhwfw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmxpaalwr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gclwsedee.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gguvwlwod.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gmmvniqxf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gilgbijes.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gaxijxpyn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gpianguxb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghehgambf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gtjmiguxr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gunjubogq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gipmjwgeq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gpogdedyp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gjtqsnmec.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gvxzvezmq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ggaeguxoe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gmkjohxlz.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gecgkyxvt.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/ggsinqmtf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gqmjshwou.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/ghdbgqskd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gxzavomed.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gvpceocrm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnvzcsnow.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gksppbzvp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gdnicpskh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gdkrbkbvm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gaujskguo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gtbdaragb.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gffwchnvf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/giyacuixa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gwbjrszky.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gnnzhtwqk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtsdjpwbx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/guzkwlvec.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gpmxcfinh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gnifvhfif.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gvhldqseo.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gbjwbtqeg.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/ghejaeqey.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gdgvadsgw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/grofzhxyo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gatmorscy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gkbxjaugn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gryzqirul.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gaxoiuwib.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gxptmyrde.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/ghoyodyeh.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gdmsdzsnx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgnzfakb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmzvaipiv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gzahfrvhr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gvwiydcmm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/giowwfjfi.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/ggwijtahu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gkmiurfwd.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/glbkxwhsf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gplynahcs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/goacgcsio.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gvfblhhlk.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gmkfdvhtb.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gkgfalagm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gwqtdvqse.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gycepszhv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gtnixnqoa.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gibvvrhdh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gfpphluvm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gsaduxtrf.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbqpgphdk.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpahbaxci.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwiwconja.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkxocjlqp.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/ggpeoztne.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/grqtdarjx.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gvdugbjpu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gxgoaubik.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gizbxsujw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gpmgnhqsk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gpwnkhbyu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/ghhiifofb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gyigqvbag.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gocggseay.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gtanqqynt.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gpieekbqn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gnopbigiw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gtbwjhzar.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gnngviwzq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gndkrstql.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gbexpodqe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gbahcptqr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gyvxoxjen.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gbgzpmjtd.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gisyghugo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gtpesbncz.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gkpuytmfi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gcqarbzkw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gfoeqybby.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gjeqqbnkw.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ghqfrklag.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gbqxggljk.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gikzoleqc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gatdtqqvk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gvlfmcogi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gcfuvaged.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/ghulbdbjb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjkmwplzw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gmrranllh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gakqgrtrr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gkqmcbjed.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/giynbykbw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpplgdnnk.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/glkzldyrc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfhdihioe.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gdnqltkcs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gyvbppkvw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gwfdotigg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gcloeihsu.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gkyzcddko.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gyqpyvrei.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gijdojkga.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/ggkrjthew.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gbjjjkmqy.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gqijzlulz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gvnawhrvx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gplviojfl.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/grajfanek.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gqaqgfrpc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gtcbqngjy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gbdssnjgd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gftvbnvba.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gdajekpiq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gykznaabg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/glhtcvijz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/glizlwbrr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/ggaofvosy.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gaeuxxjex.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gtkqwtkka.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gmwihsgwa.sHtML


<!-- 参考信息 -->