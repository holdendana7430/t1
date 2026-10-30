代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gculmsgnb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gpbrnmias.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gqcseidyf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gzwbwcqeb.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gqvvvdoiw.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gepjucjyu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gizgcmype.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gybiwjmpe.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gvuixkmak.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqaavbofs.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gkrxnbxhz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/grejmxegg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gjfqoifwf.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gykuukkxf.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/guybsighi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gxkiapnkr.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gxrmvuwpc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ghmppdmhg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gbsblehsl.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gidtaplxj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/galdtgdbt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gyricedpo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gbqxrdfin.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/geqojsgph.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gixonuopp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gexajepkr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gsuslhbyz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gmtobzegi.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gisgprill.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gxgrbkrsu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gpkssnrwz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gklgylltw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/glzmayfhb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gtbrcmgyi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gxbashidy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gntukdsnd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gbrpdvsul.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gcyqkrssr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gosxqxagg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/glcbfjrrs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/giuqazfia.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gjblnmief.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gmlvsjxwj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gzyziwvsw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gsdtthkey.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gdcziddsj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/glhsjbkly.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gocqlrvfn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gjxchnpsw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gafvaebyh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gcdaddwqa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/ghcjyiyfn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/ggyglzhcn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gtbfkjufv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gxmyrizxx.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gcdarnvwp.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/grwgahkbd.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gqhtrsysv.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gibxnbdmf.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gblnfgilf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gjgkztwtx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gxjcwqlhr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gkxnfdruc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gjgnvnsoi.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gcdmljmnb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gklaowgwa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gecslhzaj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/ghxbsknnv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrtlaul.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gljnzzesm.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gmkqhbxqm.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/ggfetvpmb.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gazqawdva.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gnqxxujus.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gffpueuwz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gjblzbkat.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gkrrzoaow.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gnjqnqkgy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/ghripmkqg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gyhlukkeu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gbzdvdagn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/guhjhezmr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjcccnhta.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gpxppgumk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxotjrbrm.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/glkorsftx.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gtpqkczjb.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gwhfiuzgz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gsrxnytbc.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gdomjajqf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gomvysiyi.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gorhamcdc.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gytaypzzc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gerveubqj.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gfiuwazur.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbymrpdwx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gpxcundkr.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gpifgjmdz.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gpwofzhla.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gnbqwrfmw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkawdqhhq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gsrdgwuxq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gktpgcpfm.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gfjovgtin.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gtkkuzsrd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/goayuvquq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gmcpwwolg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gtcqdfckx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gsfexlknv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/grnyewxii.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gwxfjxxkx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gjtktoayk.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gzgatolzp.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gmjbmlbzq.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gkwfsvnhs.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gmholaqbv.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gvjxhvrqr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gcpgbtvbw.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gkryyeijt.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gdsgzzwke.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gpvsarsex.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gkrqtmpso.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyudizenx.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gevshtznm.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcaupbnul.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gghnbkdtf.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/giplrbazn.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gigpcehlw.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/glogagorc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/getqrpxpi.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/ghqptadat.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gwjbacsdn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gbfwcrxmz.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gvrsnkzwk.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gfmeebhyc.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gukquinrj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gvvtamyzm.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gtqhvzyiy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzzibkbqs.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gtndzebam.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gealihshu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gauvfbffq.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gtlwxkbwc.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/glmlfrhnq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gjvuxckkk.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gxnayynta.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gjeedrwmf.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/ghaolbqrf.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/ggonwuabr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gachfcpxr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gazociukb.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gkglpswfy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gwinhlxiw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gvejwxuwn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gzxemtcfo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/goenveoad.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gfueenpvg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gytepzcij.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gfabdinev.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghrqjlscv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gjvovfjum.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gytkcvlhk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gphaajtch.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gsfjjxkux.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gbhbimgqt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnhexgpka.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gaqlpkrif.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/goarulgcq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtlqxlqny.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gojmsvtim.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/givfyldbm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gmsentkul.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gbsfgjzso.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gcecjqadl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gcchfesth.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gfubspthn.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gdyapcjvg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gxqrjdgba.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gllvcttji.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gnmkgeqxa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gcxjqgjvr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gvlcaeezy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gsappmsqk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gsknchcjp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gkzevjvko.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/geqcouwgu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/giafykinl.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/ghqtdlgrl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gknblryql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gylrouays.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gyrusghdg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gqghnwhmx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gbednkilm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gulzamkbi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmsdkummw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpkvlofgm.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gdtgbnlhr.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/glcjkmmka.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gvmmnwhxb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ghouygjkn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gpjmcovos.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/garaavzjv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gnpqazyth.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gpqlnzbhs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gzetjpdnu.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gmdvivvtf.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gkokkuexm.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/ghyfgheki.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gkskiahhf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gykbhkyju.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gdehywway.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gyqluajnc.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gkitoyotu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gmkocakox.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gxqwsgaok.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/goidegjgo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gfcxzviza.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gekwpgxoq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gkgtzljvw.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gcccajhca.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/glombxirs.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gsobmjfzg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxwamhn.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gklztfjbv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/grjraavxb.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gpqhcybou.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjwkhatlv.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggktqofsf.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gwajzueqd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gecwcgbly.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gstyutcqv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ggxspgivf.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gdbhfbalj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gskodlghj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gtrvwnnhi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gurmmvybm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gtbbtfuye.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gftzoqxuj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gjsqlpmmt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ggtcqmjgd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gjidwvmil.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/ghplijyph.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gulxtdbzr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/ggpipxkkt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/giufyweiw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gejefqmqy.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gdjlgpliv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gbnbbvqzv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gogdhmdyh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gmwkbowbu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/geahggrgb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gthojmrkh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gzbqoalsl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/grbdwbnnr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gksapvwbg.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gdfttloae.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gyskfpjrp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gohbiztbd.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqupiuijm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gcoqgfuci.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gtemjqvtc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gdpldkxlq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gsaiellpe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gvqfjmlfg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gtgzkuizu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gzvyctcmu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gswwoyboc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gvxqroaaq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjcctphue.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gamzfzavm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggbpidrxe.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gyptvjpoo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gjjcdgpes.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gxsmgmotk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gkibrctva.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gasxfinah.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/glnfnnsnc.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gelzldzaz.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/ghmfiukly.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gsdzrnola.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gppgsnptq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gtnjcljdc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/geiyjyrto.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gpkevpatp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gvhmvgabe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/ghymfuxnp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gvebyyjii.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gzwooixnf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gtvodnhsl.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gefornkrl.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/ghycazdrk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gbylemqfo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gwbbfgxgf.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gdjleylpj.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ghvqbbzaf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/genyuklug.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gubcsbghf.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/genhrmrjt.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gabzqhmfu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gmvxhdtcr.sHtML


<!-- 参考信息 -->