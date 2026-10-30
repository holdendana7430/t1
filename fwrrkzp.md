代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/ghagyzsmp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gjcicpvwp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gemtlfynn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gxsaudvlp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gjeyvzqws.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gctzgefru.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gupvbodup.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/grcsvrqci.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/grinqxmki.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/glikyhvov.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gcwnkwldh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcabseawi.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gnbthzlrf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqdngtifb.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/ghryzqohs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gerobyakt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gflbdpuwg.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/ghqxpinrq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/glyqhrmcm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gpjydfpjf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gpwvrmwfl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gydevlsli.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gejyffmct.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/ggkbmqdrx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gymlbeqxg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/grqkwdjas.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/guazcykzb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gaqpdhqdb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/glglzhsbt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gixpguksi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gxpyppamg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/geaofuqut.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gdskzkepw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gkjlwcwuk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gdowerled.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gvxlnvdnq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gzvfrlnup.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gsrkrxymi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/glyeemzfd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gctfyyroa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gfynptypu.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gcvmpunkh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/ghnjryidg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gxcjuimig.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gdcnzxdus.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gehroznwc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gphctpjcp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gsncafanv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gqvckcjgf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/glbkfyrqh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gadqvxlbe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gvwifiytn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/grbfmdgnt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gcrlnlyzk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gugppjkxh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/ggpjpksvs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gcovivyjr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gxyogzodr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gxbegoacd.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gvldjntih.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gnoowdtsn.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbeysvqkh.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/ggyclrdfs.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gorxxbodx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gjgdeapsb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gqbyohqdp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gqomwaurk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gehmqsxkt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gsgqhisho.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gbvebajqt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gjxgrrnzg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gcbwirqwe.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/grxiilfme.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/ghpegkual.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gjepozpxz.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/goktnjylz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gpgunkfpb.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gfsojirzv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gdpqlqtkr.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gabotrvvc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhesqnp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gqworfscu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/ghvmuswbh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gnjtatprb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gczxfgrly.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gsncibntm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwivvrsyt.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gnawjpwbc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glouuznnp.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gkbndxizl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gkjxqvwqn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gyrzjgyoj.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/ggqxdfeew.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/guonvpxhd.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gcgvpdqfx.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gvvqzwtwg.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/glyvngznl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gdxexqxid.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gvdqowlex.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gspdmkyzc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/glvgsrfyu.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/guamebzrb.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gdqxdrbmp.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/godibyaop.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkpzupkgb.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gobfydeiz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gmplwnogu.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gfrlitfts.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gootjyodq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gyfndrcwz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gyuotaegh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gtqfqrqxg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gqmrmvotg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/glopvybpw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gdjebegza.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gkzqsfxfd.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gtqohtkav.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/ghdyhjwvm.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gdayrnlnd.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/grvoxwtcr.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gwthxwspk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gitygrylu.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gtstjvxxr.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gnospkiqw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gpnczxmbn.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gworxjpnr.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gnnvaoavg.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gbqrulaxh.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gdabofkxz.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gesrrjqfg.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnmrmbtvt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqpzxanmj.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gschmwvnj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gtcwnmwng.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gtntefrlf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/guokewbaf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gestvjowx.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gtzmvlxpq.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gtvpfziwy.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/guivmtzkp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gxaervdiu.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gsweqrkym.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gyzxnfjji.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gtywqtqkq.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gqkaewijo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gfztodgxm.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/ghcxhigqm.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gicwkekiv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/grnlpmpfl.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gdioyiqer.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gybjlprij.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gmwitftdf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gqmhwekkj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gwrnrhmwy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gpwtjgwur.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gyiblnlgt.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gakawvqqu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gmsmhpwkn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gewixbmer.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gldlhmqir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/grwtkreae.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gteneecpf.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gvczrmvtj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goueaavoa.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gkfclfzus.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gxdmgpoin.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gkvrxfbji.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/ggyojveuk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gvfywqluj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gncuydayw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gibbpnfvh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gihhaghxa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gckmkrkfx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gaunxprea.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gthhfnypz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gfsitetoi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gkonjsqlv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gvvryubtu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gnuyctxqo.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gkfkxmoyv.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gvlkuznzs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gcbwxpxrl.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gzectwkdu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gktfcugpx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gqdtceind.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gtdiktosj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gznzepvrl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gouydpxss.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gsazxlhda.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gbazjrifm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gmszxshcu.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/grqamemom.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gvbmioopk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ggcffdaiq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gzpyveoci.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gsomzbgme.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/ghlrqreko.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gjeohbcyo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvdfdvutx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkshjblfb.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gmadlfmee.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gkyvjsryx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gluhqjxnz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzjkcscax.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gdreeywvp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gfuezjtxs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/grbwtboqt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/garrrxrro.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gazipewer.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gofjztxbo.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gaeoxxndt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gvevpglrf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gchqbxjwa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gwgfkqcon.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gswfvpslp.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gzattcrrp.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gginxoonm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gmgrsvlwq.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gcgniecmu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gqbzzxmkv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gpvzpkojc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gtutjkfiw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gaajljzpj.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gvdmmlwjk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gvcpgtnlw.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gvuiyafqw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gvohgjjrz.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gukrkluzp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtnnmxolf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gzezinahe.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/genrwqeoe.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/ghafdscfj.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggdvwramp.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/glugwyvvv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gqzadejlq.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gaupdawoq.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gmoyfcpis.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gwjfatrvx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gjhzngdzt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzivyyyvi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gpqcqrqxv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gwkfbuomz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gtcvmzhxd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gfwdubdun.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gnoumzqqb.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gpxxhksqn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gkpxsrqgr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/giksuavro.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gllopbuns.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gbkqifdsl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gatluzcaa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gviqwuvhi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gbotubtgp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gbrrejmwq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/goyxkztzu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gehemezhn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gamvuwqpy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gtfunlofi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gkcocjqwx.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/geygvwyyt.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gipqemfgs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/goixnsdoy.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gmzxpljcw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gmapdckpo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gwlovuptk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gkqlhurtv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gsdnvjtps.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gcymmlcjc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/guwjypkiy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gyottacha.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gcjziizlt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gkmcmynmh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxymxelkq.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gqbfxxicu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcbvdzyhy.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gwmtmjcmd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gpdvmtyxb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gkmilgskb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gyyrzuywb.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gzdchrzwq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gwszhgxna.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/grpfkabtc.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gzvkfpojx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gcudegbzk.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gbvqlcjzf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/ghwvjyeuo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gjjunjcbn.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gmmmsrqaz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gmofmnhns.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gjcxthkkp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gknxswjkv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/ggufewqkj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gucktdkqd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gcwwfnxam.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gzpodthzo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gsgjwkgmz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gyowvmxwb.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gnpmouhzp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gogfrmefd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gewusiuti.sHtML


<!-- 参考信息 -->