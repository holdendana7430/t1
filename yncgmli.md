代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gogdswxwl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gtnrpkybd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnacthylq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/ggrbdykoo.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gqgokwahd.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gqkuntzvw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gjvddfdls.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/garxiahvy.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gtfrcvkul.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqjiovicc.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gvqdzjkmj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gesggrzmo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gdgwqfbrd.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/ggemmdbcg.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gfcksjoax.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gbgymbbei.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gohhtutvn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gmcqcnuav.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/grhxumapf.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gipwrweza.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gjnfoklps.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gijekhbst.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gdfdnzmns.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/goqnirpov.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/grxrtfmjf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gwvtpknma.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gzwayzgqn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/grqbldtch.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gwxgrjewy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/guewvztbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gxgrjgyos.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gzfxmgwuu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gkaqjnzvv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gnijmizxl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gyseehwhf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gtnquitbd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gvdjzopdm.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gpknfxhlo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gkkwdyqxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/ggykptyie.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gyiojrtcc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gckwybzzh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/guuaapkoc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gsiroeuyr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gpkdknzzt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gjkihsmgm.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gynkufnru.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gvlfibrga.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gdcthxisj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gdjdmpkyj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/ggbrtabrk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/girtavpoh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gvgwgteog.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gvnsddico.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwgflurie.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/ggfgmjzxq.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gygmltplo.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gdzkdelaw.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gqgovmpsa.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/grzzmmpev.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gjirmdiso.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gapcxcmsb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/geeelpurd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gkdymgsrd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gvfalgunn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/grjrbqqqe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfuuhwdv.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gegxngltd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gsszbopof.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gbqtlyexj.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/glifzuyys.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gyojygqtg.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gvdbsmvpb.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gdfoeqkob.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gaofmwiiz.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gvjccwqsz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gfrhguybm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/ggoasefya.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gfbzvndcl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gkwjqpmkm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/glynohhbj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gpfuysicp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyzejxbtg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gwgxvgfqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdbfpgymu.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gfzerjgtt.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gokwwydze.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ghrejxqjl.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/guriumzvb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/galjoicet.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gosxvqewp.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gwsxlcskl.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gszdofank.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/glvexquij.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gaqwgukbl.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/grcbpgvli.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gboeensgf.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gdkfxyedz.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gwezvoonc.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gsopxinmu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gtnjckkcd.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gkldioqku.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gilzhfsrz.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gkzlydjel.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gmgunuosu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/ghjattvuo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gyaflevbo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/goxqicnnl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gnlimchwt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gxrupkayr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gbpeyvysg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gnfndmrfn.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gzvnwewlq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gvnkvxykf.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gepaypvox.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gepdjbmnn.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/ghbohutpv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/giaigcakr.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/grnhyzpnr.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gueraxwvv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gdmuxujxl.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/giscxgesm.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gpsnqawbd.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/ggrocdvcx.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gqnkcgjzl.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggkjfxfua.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/grxuuwqza.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grqtnqibs.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gpvrzujen.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gelyhobei.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gfyqhzkhj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gewrvaryo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gxpzvglii.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gwszseabg.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gtjeywxhu.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gpspdwkzz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gpbetylst.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/goijawfld.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gcqtmterm.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gknfdyilr.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gwzuyhxas.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/ghrxgvvkc.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/geyyqyjrb.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/glktlchzw.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gjgncuboo.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gzxeakrtl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/grihqdous.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gmbuvquxi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gnyvsvimg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gtggvfqqe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gqjrcxfuv.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gqsnzqajp.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gampqcwkz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gxhimeduo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gmfnhisvd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gnjfllizq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gcvswivzw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gavmpyohj.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gcfkksejo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gejnnqted.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/ghpgzluap.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzafwsffm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gwtoqyrsi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/geztweala.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gliqwmndk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glbyhncmm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmulykuga.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gxmwwksyr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gjqhpabnx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gqjumqgbm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/grsgundvu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gfgzactvi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ggyoboqhy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gaaffwths.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gpuoirgep.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/garhfnyzv.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/ggsnryqtx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gcxmohglz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gmmrbhwlv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/ggyjgfdwx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gjhmslcwh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gjhjsrxxu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gylbpvvwl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gfharjrgh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/goutjtcmp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/geotqunft.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gzshtxrca.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gdolpvfay.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/guduehqdw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gcowihnfy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzzhgikxu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gdmunaltx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gqggorpze.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gbfuugwfv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/grwtpzftp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/guodfpxff.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gyyqxvbqg.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/goffvvuiz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gucuvowjg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gqpgxsymh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gnklyghiq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gswsrfngm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gcexmkhne.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnspynxab.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gyudjuzyc.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/glpibgmsz.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmtqhqe.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsypeupol.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gadvzzlmn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gbfslxzcs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gtewnibux.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gualkckwf.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gxrwqdypr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gqcdpgjdg.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gbercxotz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/ggxokecta.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gwzgttosx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gjzlthwsc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gplbopqby.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gjoabvgvh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gkracgric.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gltsxnvep.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gurseponu.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/goqhnqivb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/geapndjpt.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/grlunmnzy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guxpwimxi.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/glbgwaihz.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gakfdkkjk.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ghvhznnzg.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gbuxjvtrh.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gfxmrzlet.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gtlzobmnf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gkhvbfuxm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gryfrwumk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gajgotwix.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gvirzhwxc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gjwonnfte.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/guosedspf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfijnpcyr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/goepmokam.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gekjywena.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gsydvnudx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gcpxindsm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gprmmujkl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/ghsttfhik.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gggroalcq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/ghuenksky.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gmojjnkrd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gozpambtq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gpjhngjiw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/ghmfjulqp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gcgdjofqr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gdnhpswhk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/geglmgsax.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gejajxxsp.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gnazbnlib.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gujvocvrb.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gvbudstjn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gpxcckznc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gcczaewly.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gzvvuhsxu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gabptxllo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gdnwoqoyg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gtsdumfwg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gqevuynnu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/galzocwrx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gnkoqrfui.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gikqftkgi.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gqhfigtbm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghfxvawzv.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gigpzezxv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gahgkzbgc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gughxvesv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gnnnizsir.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gtwejcylz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gdceqkoqu.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gejjthkgx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gsucghlqi.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gohehhlmr.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gxiljqadw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gtvthmbra.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gktisvdnn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gezhgxolf.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/govpcbszk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gctrndxih.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gzsfngwqd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gfffmjnix.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gwlkjokkm.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gjzclcrwl.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gtzkhtngs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gglrfflrj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gdrqviryy.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/grawlstqy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gjxiyajvp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/glxomsfqv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gbhmtvblu.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gazbihxqy.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/glmtflfew.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gpougmcxj.sHtML


<!-- 参考信息 -->