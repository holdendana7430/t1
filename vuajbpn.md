代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnissfwwv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmxbmhvz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/glsrxnzuu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fanxiaobao.xyz/Article/details/gdcqyxgnv.sHtML

Go:   encoding/gob
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkvccgfg.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/grnmtwftd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafwiyzyz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govkyzrxv.sHtML

L. 网络请求
来源：http://blog.fanxiaobao.xyz/Article/details/gsjwsxgfq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gizdvxhue.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/ggatpgiod.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbaqwzcp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fanxiaobao.xyz/Article/details/gbauteyxb.sHtML

JS:   await fetch(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gtiohjsmh.sHtML

TS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/glenvxbet.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/gghkxtlyc.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fanxiaobao.xyz/Article/details/glmmhcfhj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/gcdkvgphd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gximfnqll.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gourjbwcw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fanxiaobao.xyz/Article/details/gxqzfwbcw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqinashe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwbqwwmu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gpytsjscy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqhduqvo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzlslche.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwopbium.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/grucfcrip.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fanxiaobao.xyz/Article/details/grtlqnsix.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fanxiaobao.xyz/Article/details/geyzzspmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/glhvfiuxx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhurdyjg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiqngqtw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaxspplk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhmpnqdy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcurtgpxx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/gaforekno.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/glhbfswve.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwaovhpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gyhdmyjvh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/guspzrzrz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjdqclhp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gpxiqyqtp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbvlqslv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gzvxtranx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/ggwlbgtsu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giafzfvfk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fanxiaobao.xyz/Article/details/gytgeentf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzvdfolr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwuxhkfv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqfwntvd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/gurdfdmop.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyqctdeh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fanxiaobao.xyz/Article/details/gzvjnxuxg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gzomsqplq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/geoyoxjuu.sHtML

Py:   resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gkfhbnuhd.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gxpovygjn.sHtML

JS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gbnyfuasy.sHtML

TS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/godchfgqh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gepkjfpah.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fanxiaobao.xyz/Article/details/glpwwllbp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fanxiaobao.xyz/Article/details/gbodxnxee.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gmdmivvop.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjauockhn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fanxiaobao.xyz/Article/details/gplucuqpr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvsgvjyg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/ghthfntvy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcsqufxy.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/golepyyzy.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggohyhcpo.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsiravdr.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/gdygbjyko.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/gderqdutr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdqsgigz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/gipfcixdq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gendhvgxb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gywmvltrp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/geczxnsno.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fanxiaobao.xyz/Article/details/giiilpxmd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeuoropw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gognxlkhc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggqenfyzy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvihqurv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoqqipcu.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gtxvgczfo.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gvisdfiwn.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fanxiaobao.xyz/Article/details/gzlkovyzq.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtfpkkn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/geepvuyjf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/grnlzolwp.sHtML

Go:   os.Args[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gzsrrzakd.sHtML

Ruby: ARGV
来源：http://blog.fanxiaobao.xyz/Article/details/gzbviqojc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/giyllwzgm.sHtML

[M02] 读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvenvndg.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gvshtlnfp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/guqjyboyb.sHtML

JS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyfvjzaz.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/grsigtlmz.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/ghqqineqe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqknkhgmt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fanxiaobao.xyz/Article/details/gcuanrwsy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/guqftmxxx.sHtML

[M03] 执行外部命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdglsoog.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjfjkuuj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fanxiaobao.xyz/Article/details/gsgmaqssf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfcwvppi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gmddbmzsm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gpxtanoyq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmbnduvz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fanxiaobao.xyz/Article/details/gfnsfovmy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gigydgzmd.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjxysmck.sHtML

Py:   os.getcwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsycalsa.sHtML

PHP:  getcwd();
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtldeghk.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gezgfhvtg.sHtML

TS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/guqwpazhe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fanxiaobao.xyz/Article/details/gcbesdzhr.sHtML

Go:   os.Getwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcippuox.sHtML

Ruby: Dir.pwd
来源：http://blog.fanxiaobao.xyz/Article/details/gwotsavcl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbslyrwl.sHtML

[M05] 设置退出码
来源：http://3g.fanxiaobao.xyz/Article/details/gcfohluqi.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghibkvszi.sHtML

PHP:  exit(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdulbdgen.sHtML

JS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gywrllhtu.sHtML

TS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgxfogbt.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxeupccp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoludcvv.sHtML

Ruby: exit 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzozrteuk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fanxiaobao.xyz/Article/details/gvilcbtrs.sHtML

[M06] 向标准错误输出
来源：http://baike.fanxiaobao.xyz/Article/details/gfircejwo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxsicdby.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fanxiaobao.xyz/Article/details/grcigfsap.sHtML

JS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvgtkflu.sHtML

TS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gxaumybju.sHtML

Java: System.err.println("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gdjzxzksa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdltnrki.sHtML

Ruby: warn "err"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrxyxjyu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmpcxeob.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbfikszk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxquzenf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqgmkkuy.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gcvbvjcjy.sHtML

TS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gepdrbopo.sHtML

Java: public static void main(String[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gvdxkythe.sHtML

Go:   func main()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaapesps.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fanxiaobao.xyz/Article/details/ggjwnjcov.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzqvklns.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fanxiaobao.xyz/Article/details/gqrxtcfbz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gguibsyyc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fanxiaobao.xyz/Article/details/gssjgvvum.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/ggpfezshb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrtweayw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/ganizjtjp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gjmaopjwh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaxftorg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkcwhvae.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyssssmas.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gmgtczojm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glxmyjymv.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fanxiaobao.xyz/Article/details/guaehnnwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guihfwuuf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gbmgodtyd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmfsshaf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gsxhcisbo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaqxwaum.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/giybqrkpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guehuudyl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpwjpaus.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmyyyfms.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqclvsoi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpepfexuc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gjkypbpkr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/grlhubsyw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fanxiaobao.xyz/Article/details/guihbeilv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/galjkjwhs.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/guccsxhnv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gnijpnhck.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwtyrqkp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gytlyofgz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fanxiaobao.xyz/Article/details/gljodezgq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpdyrdbv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gubmiiqxa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbpiabcy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fanxiaobao.xyz/Article/details/goewfclxv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjmbhxkz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyrljrzp.sHtML

[N04] 斐波那契数列
来源：http://blog.fanxiaobao.xyz/Article/details/guwrzxmli.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaketcik.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfbpyilrq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/guuxurqqn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfsuqllv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/gydmgllqo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvornzej.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gezejbeji.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gklotnaff.sHtML

[N05] 最大公约数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxriwtvwa.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoitsyrb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/guefpegbc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpkcgjuv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoymdzhi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fanxiaobao.xyz/Article/details/gyyrrnjqc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fanxiaobao.xyz/Article/details/gottvspye.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbbzoxar.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/gejjaqayz.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gsdgzxaxt.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gtyzjtsks.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfhbhndt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjknrkasg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqdmjjpl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fanxiaobao.xyz/Article/details/grgqnlbwd.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fanxiaobao.xyz/Article/details/givnpycgq.sHtML

Ruby: s == s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gpwtqmnmg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnalmyxmo.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gugjensss.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiqcoxcg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkhrldyg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvubppyxv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxjtgxup.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gafrulyef.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fanxiaobao.xyz/Article/details/guuwepauj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fanxiaobao.xyz/Article/details/glxnulvwp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fanxiaobao.xyz/Article/details/gywtpveam.sHtML

[N08] 生成全排列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbasvspdj.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gkluxachp.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fanxiaobao.xyz/Article/details/giknnuaua.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjaglseq.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwfkeykw.sHtML

Java: // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/glptmjebc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxznozbb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gggbptbgu.sHtML

C#:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gklglektb.sHtML

[N09] 栈与队列
来源：http://mobile.fanxiaobao.xyz/Article/details/giynzhpmh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/giydtexkx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrtvbspm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/grnjepsyn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gykccgwag.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaedlgmj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/gagajzfth.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfwqogke.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbjxzqkq.sHtML

[N10] 链表节点定义
来源：http://blog.fanxiaobao.xyz/Article/details/gypxpaewe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fanxiaobao.xyz/Article/details/guzognbbd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbkuzxmr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fanxiaobao.xyz/Article/details/grdplglvl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnhfyvmr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdprrvs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrwxihzc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfpzhsqj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwrixkzx.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdufjhjlb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fanxiaobao.xyz/Article/details/guchfoypg.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzxcvgkrp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgiqqyhs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrusifkq.sHtML

Java: // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gmknmtyyf.sHtML

Go:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gwnqakbva.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwzqruig.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaomtldwm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gwqxdpmqy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gygojbqdo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/gormwdgzq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydenvuep.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblklptjk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidnexslf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fanxiaobao.xyz/Article/details/gbksiunrz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gopywlqaq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsuwmtdi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrahsrdu.sHtML

O. 并发与异步
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpocclnq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicefecbb.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtrruztu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoylljok.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbttwsqfq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fanxiaobao.xyz/Article/details/gehqelqet.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gwiuyxtsc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnknilqek.sHtML

Go:   go f()
来源：http://3g.fanxiaobao.xyz/Article/details/gmydocwxl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fanxiaobao.xyz/Article/details/gajbbylfh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/grfrsxbnk.sHtML

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywyybreq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fanxiaobao.xyz/Article/details/gveqmmmoz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/gsamzrdhq.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gcjshkgqy.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gskrdezlq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjcitegf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fanxiaobao.xyz/Article/details/guwiaxaxb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhtgufop.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fanxiaobao.xyz/Article/details/gtjmuufgd.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fanxiaobao.xyz/Article/details/gvnxeszrg.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcquuqcoa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fanxiaobao.xyz/Article/details/gnpqbwyng.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkdazdvf.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gsixhdchr.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnqzyzobe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fanxiaobao.xyz/Article/details/gizrskprm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnaawlbp.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxmrhxyyo.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvvrasqe.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fanxiaobao.xyz/Article/details/gxuufhoxf.sHtML


<!-- 参考信息 -->