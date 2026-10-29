代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/grssudodp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gcsffmfeo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gzhqznugz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gyejzkkwz.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gtabktbyg.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gtntayepo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gyfvomsln.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gacnjjyyc.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gowcagmyi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcccbhgjy.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gqouempfw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/ghqdvekrx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gocugwxpo.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gmdizeush.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gpuzhqwhz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gdgwyuumu.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gvxvbbsoj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gyucsnewu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gbjxhvvdq.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gqfhtxmpc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gpwprmhrp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/grwcxcxwm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gttfhucmc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gkfjsmhlc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/grwvoenzd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/ggkslmsjc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gvzzqniur.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/ghaigvfmc.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gzgdhnetq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/geqqvrtal.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/ggbahdmbp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gunlyvtej.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/ghpjnvepu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/guipqndgu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gwmooqlrf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gfktkgvwk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gwbfjavpv.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gqjpncdfu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gjiichrwd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/guvdykqay.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gnqmmzumr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/glfcchwwh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gxfulfzey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gfmgpeqiy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gibjcsjdc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gpvzhpplf.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/geiltzowj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/ghscfsdzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gsnubejah.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gopmpqbqm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/ggodxawmk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gpxhjftct.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gfpigryvo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gvufzrxds.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gyfqxqhrh.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gbbetbgrh.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/goiwxdkzh.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gkgqczoao.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/glwmmqfdw.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gpkhkblyf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gcipjtqdw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gfkluzrud.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/ghapankya.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gjnzvdndz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gdudkoifa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gkcmitaam.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gdppbctms.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gmxkwdybh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gazcqslie.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gmqnrphgf.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gudvgwlie.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gsmyovcdj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gngkniybi.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gavnchtez.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gmuvnieoh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gwajvvcnu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gcforimlz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gsmvilynx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gjbiebnco.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gqgtrncey.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gwdoigons.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gfihckdnz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gptkcwyjx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gvrgflaon.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gylrzzfgm.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gzxsrxgzz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gryxrkixl.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/ghexittya.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gthojxuqt.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gtxnykggk.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gqdrchuob.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gunbtjtqn.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gnbsusflu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/glrmmznvt.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gtythppwg.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gormvlhoq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gljzikpza.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gnrbegnwg.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/goqhujjgo.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gvijfqofr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gqsxmibfm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gepfhpggo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gljxaooak.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gkdbjtolv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gfdvrupbi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gxjxiroun.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gjjmtmarl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gacbwvgdw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gupcgkguj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gxyytpzkd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gxbzmjpsh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/giekrvfcx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gywbepybl.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gxtlokgbo.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gjamfhbez.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/goncrcjpk.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gcjgqepxs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gudoaagvr.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/goxnfggfz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gjginybnc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gfyvloawc.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gjbpmaslp.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/giurkxkri.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gugmshlgf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtoyhkfz.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gykjakznd.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcjdlzfdw.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcyxlrnkm.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/grgmsojmv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gwnbmgedh.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/giflcnsmm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gqoxmgzza.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gycdijoyb.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gkgypxxxd.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gqtdakjpk.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/giowldgzv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gmptyxfhd.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gzplhrtus.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gywnmrelp.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gjotmzuwo.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gxbnpkroq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gspurpbdd.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/ggzsyoyre.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/guiekevwb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gaqefdndp.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gvuqflyhj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gwrhjhlqa.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/grlikusfx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gxamfvrxx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gvuggasde.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gcfshpaho.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gqlqsevht.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gxhbgympn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gjowurraz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gldqetjzt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/giwwwuxso.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gmcnwziih.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjhipoddz.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gasjullpi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqmwcrfeo.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gitsdcixx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grhrueduz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gaslzgscl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gazxfbyxd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gvveufqty.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gadfyhayi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtzysupkq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gkvugxdok.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdysigryg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gfznphext.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gooiwrkmm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gxwkybdkv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/govtnkegu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gnzwstqwu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/glbjbxahm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/ghykdewvh.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/ghukbijbe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/ggionjvqc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/guugrpfjd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/ghqlfuxrn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gcdzvniao.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/grvzxtimv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gkyedxqdm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gndguoowu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gesfujmjy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gcxpofplw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gjvleoomy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gvpatzkif.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gtdgxummm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gcddagqes.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gkzdioiwx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gsavjjlbl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gvbtlqkwt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gyykhjvjk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gratpikvx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ghkzcwtit.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gnazqqxai.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gcrxfzjeg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gqdvjgadz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gglkuaybb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gqvcmblhq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gqcwakjbw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gjhaghhid.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/glcrnsosk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gtgefqzkt.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gbehcifok.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gdgofzgpa.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gowrzpvzi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghfhxuhcl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gpfcqiwrc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gypsiymrq.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gkgrhgsra.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gfepdxirs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gdhataefd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gyqrkqdrk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gflkwakqm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gwnusmljk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gnxxggnmc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gnatwdypw.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gvecmiggg.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gsicxqhvc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gfdvoyutj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gaedrxpxk.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gsgrrufim.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gxsbuhlsy.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gnuskkmht.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmddbpuwk.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghmdpmmpp.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gltkmouip.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtjxdxedc.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gckbtaysc.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gfazuqgcb.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gkcaocqxa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gjpavqaoq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gwlzatgvp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzqvjzzvv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gvaogfxgt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gfgdyrajt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/grgrjzzvo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/glqosprwe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gpzshfswp.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gnltigbcj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/grxhnjdvn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gawhcjenf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gphltntfk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/grouwzbjm.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/ghgzqhjkj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gdluqrsme.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/galwrqrus.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gmwtrwqyp.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gbobnzwkc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gbjrfqyqg.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/goisscinh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gulhifxvp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gzpamsucn.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gbykgsroo.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gihbohtvg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gjizzbmea.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvsodfwph.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gbdyygmua.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gqthsctbl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/goquqspjg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gahrplydx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gwfxawkfr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gvamkpzpk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbicjscuk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvciymjzb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gihrchzuj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdeckbaau.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/guiqfjdag.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpotijsqs.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gheeqnkve.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/guwcwntso.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/ghpyahqhs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gcpeiracr.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/ghssvvtby.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gzqrmkiws.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gwhbntvej.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gyrzowxqr.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gnnwsqala.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/godbsoddi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gpdbzmkih.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gksdqfaah.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gnopbmtzh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gisfpvidz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gffqwjcts.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/grvtldtdq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gxcytrssg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gaymmqqrn.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/ghkxlaevl.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gdzywisvi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/godhypsns.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gudsczahi.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gakwztidx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gsrpggbty.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gtjggfnro.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gliovovio.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gcmktonhq.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gjtegwmvx.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gwebhsuco.sHtML


<!-- 参考信息 -->