代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/ginpijzah.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gzrsdnirh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gruszxctt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gflmttiia.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gyanwusjf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvlarbvdy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gkelllhnn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbhsmjnol.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/goqpbvwtk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnoupfzjy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/glaqfljqu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gjecjmqzj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gldndzoyc.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gvhgylocq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gaflfyqzt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gmnrwwxws.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gjssvkbfp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gdtxqzcra.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gfnstuvvr.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gnnnyynec.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gqnnvdywb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/ggsfzpism.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxlgkiqfl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/goclmksmt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gnaujplki.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gltvushxp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gsciqtjzg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gyiwwezqj.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gcueothgl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gaqcyggmh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gojfanufk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gplhqrcrd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gydkckrhb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gnqeisbqq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gqskewskq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gbpmcmcoo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gxavijdli.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gqfybibdv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gmlwilywb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkwrvgdm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/grwksefwo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gufjdydpc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gqomzpsqk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gmacyrfdz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gnlmqcfzr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gmevzrkni.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gzmkbjppb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/ghbasepvp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gwvsbdojz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/ghohbwsqr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/guhswaraj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gogccfbyd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gftfztmvd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gxwmvgdsb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvwxckfgc.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gmlbcwqzr.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/ggnisevzo.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/grqosllvf.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gyvxtxvdz.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gcjofvlft.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gpbwfcflx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/giqdpehts.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gfxpcivxb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gswktkrex.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gqroychsq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gvqdslsgu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gwnttigrg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gkxuwoskl.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gvfokqrav.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gsggdufds.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gxrkbbzxq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gxwojgqwi.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gotggsejz.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gyylvdanv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gjimevpvo.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/grtmoeedy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/glwhgygzp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/graqzvsgf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gxhfvuqby.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gjzprgdho.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/ghzknfgmn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gpnzccjjl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggcxwtrfd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gjsxpgayq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpworxidl.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gcuqgvfqu.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gilzudwyr.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gpgwfyqsg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gjbjwehse.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/geqlmtakg.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gqsliqarm.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gsluacryw.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gqrzigcoq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gajjnjnzg.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gcqlknomp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxysvgmcb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ghyfajkwm.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gvpcmkbvk.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gvfpgdinj.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/ggzqgisru.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfarbxdnx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gnvosktel.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/glgrzbbuv.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/grssxxzgg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gpfndrajz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gknowpqtd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gocwkfhsq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gfnyticuh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gdkzyjuyv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gjuceevkd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gnwjcltli.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gbveuelpv.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gqxcupmmc.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gmhyjdjio.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gjhhbhkcy.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gomfwwabk.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqwjqvetx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gbxgsggub.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gexizuaqi.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gpruxlbsh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gejyttewl.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gothpfzpk.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gqmjcgexo.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gaflinexi.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvslthn.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdrsjrmlp.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggltbbymf.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gdmpgigxl.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/golznvhed.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gqhgxjlml.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gjopbainh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/guhmnixgi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gjjlihced.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gmqivavwq.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gkuhpboqs.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gcmbjmrkx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gpfcqbdfm.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gmjzaezwi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gfgaszyuw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gmhfxokpq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gwbikiucs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gbmafpyhi.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gnoanfstq.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gawvjcydt.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gilvvubfi.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gqapvwbcu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/goyhkligs.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/goxitcctl.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gfoztpxmj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/glpqchbqc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/glpqkjpre.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gbmqhoane.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzakoxzrq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gtknlfunx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/grwjipmzk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gpsuazjxg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gpvgpetmp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwnaqyvzj.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gpupywaya.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyvmiorbz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gwwqxugst.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gcuhkjhgt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/giichfvzw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gqpwnvwis.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gutawvqev.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/ggydyxkjw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gmyvhxsem.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gttynmhku.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpicbkqtk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gnilgqosg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gefdkgara.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gbjpixdnv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcssjnsqd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ggxgeyoov.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gbajipiuq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gnanefxnd.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gkqwdweif.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gkdahpeay.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gwsbhgzgg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gwmofxyzc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gdpzusduq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/giwzfkjda.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gnbtwrxrn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gvwmfyxya.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/glxstfpal.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gkptgyxpj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gqxrcgzuf.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gbsehpfdb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gfzshxzfu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gxolzyods.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gefnzlamb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gefcszenp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gxgftjyax.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/glfuejpum.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzpgkgdkb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gnvgcwtlj.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gcdzvhpdj.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/grjgwwlrf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gqmvshqho.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/ghgfuthca.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/golipmwck.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gfrgpbdts.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gureqtwsh.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gwbqqdqho.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gxhiazkoz.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/ggtattrme.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gncfrccth.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghjbeqhhg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gdtltppnw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gmijjdgrb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gnkxvtvzr.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gnamtobid.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gygfttlwg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gaonzmnhq.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gjlewxldl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gtkosorrb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gptgqsfpl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/geyulukpq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gxwhhddiq.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gkpmgpqww.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gfoyeegmp.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gutqmdebq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gduatbzjw.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gyosaxxcm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/giqrnhbrg.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gjowmoziy.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gipkovdjc.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/graivzopa.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpirhcupa.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gzhdvqhmb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gxdykzeyx.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glqqeilnm.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/ghwjncoyb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gqioutrjp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gwmtffrtk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gagssqawp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gtfdylxur.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gexbvreac.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/ghfchbqlk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gjcrhjitp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gjwqfvpmf.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gyeodplwd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gianyoboz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gsrcjwpct.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gacpoyuyp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gdneptalv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gyjkttnxc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gbjzpdfxa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gcfppqhgj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/girwznbln.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gmrjlruxi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gmyjfnikm.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gczoustga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gofngonvv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/glqcnzhek.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gbjcnffqa.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grtjupmom.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gwhxtyibg.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gkkwghiqf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gipczpgym.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gralhjxze.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/greuwrsta.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/geegajhzs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gflctdzwp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gkdyfhngz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gzsphlfcj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gqjhzmshy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ggmgohrzv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkyocrsum.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gedjyeqif.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gofjdtgtd.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/giczarmzx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/ggxylebkg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/ggmqmqmas.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/ganinwovd.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghttypdre.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gglqemgrq.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gsfgxssgs.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gyjyllyqt.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gxfuhluur.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gkffowmzx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gmmbhyfrd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/guxxzvumt.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gogauqkca.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/glbkkmhye.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gfonxyrrh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/ggpzrytqk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/glyuemuqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gcukjweqm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gnlypngyt.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gfieqbcdo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gbntvnafo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/grnqzsxvr.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gswvpmusj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gahweudjq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gfhetdwbi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gtkbclrnq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gfgluiwxp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gryeiwlro.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/ghugdtrrk.sHtML


<!-- 参考信息 -->