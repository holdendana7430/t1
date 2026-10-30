代发 wailian999

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gcxqznqys.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkmpwpdnb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gwupawuui.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzgtajheo.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gwbijioqg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsivxuzpl.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gyukzphay.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gjlieguyq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gtxykujrl.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gignhndra.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gvgzoeihr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gjydddatf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gylojvxki.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gbxpncico.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gdxlouvbr.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gmbuxcxub.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gytvrrncj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gwhvnzxti.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gpgimurfv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gcutqzika.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gmorjpsdp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/glnxmhkxk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gkjedpgtw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gpyadgkli.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gjykvykaa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gbfghhgbl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gfccnvhiw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/ghchmzphw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/glannsjoc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gsxkzexlb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gyqttjfcc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gvopluiaw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gvwzjopzv.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gxpbkfswq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gwynnhaby.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gcgwbzzlq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gkoftteaf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gsoahrsbj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gyvqwirbi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gnlfsottz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gssjfmwuv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gadfgfacr.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gykwzgeiv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gxwdqouli.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gensweewq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gpwiyokiz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gqaciapea.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/ghyzfsjsh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gtgjusyso.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gpngmwdfr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gokydboqu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gcirvgjyx.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gnlyuornk.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gdplivune.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gqkyizcgp.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gghnntcpk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gwvhngvud.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/ghxnwedgz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gjqbmcfua.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gwsdxespy.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gibwxkkwp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gkiqtepay.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/ghbuqrxwo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/ghmmgktrn.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gcasganmx.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gphayccjn.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gmcmztqyt.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gqyjnvjaf.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gzausbopr.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/glcspkjqc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gwnodkjsq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/glkwaiwbj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gwmieogii.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggxcuqzpi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gwtgcfzfr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gchssfzor.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gmtweockw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwzvulqwi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gugjxbltu.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/grsmayyba.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjkhcyrmt.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gqecbnghq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gpackfedt.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gsqgdztai.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gyapgcobn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gzmagyjcq.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gtxwwzgff.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gicljdloa.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gfuapvnep.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gtcvocqdw.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gpwqbzcxp.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/ggiioyqwv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gixyppqmv.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gjulzfnpp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gebexhxms.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gfthniltc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gblrvuixp.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gynrpxqdh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqdcdzzwn.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gbzptuogc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gzmimvfwq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gqgwigrdp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gdaxtbmnv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gdzhwhpqc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gbhmwdlpe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/ggnpsluru.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/giorfzqqx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gglojxiyd.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gfwcykgep.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gnovgadhq.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gsoyjdnin.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gvfmcolcn.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/glqfydzbl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gxwdmwvhd.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gsacchido.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gddxgswis.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/ggtixtati.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gtxsnflmu.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gwxualrvp.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gkgrwocws.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gtohewuaj.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gezkkgzjm.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gtxhyblvn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdciputre.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gjcjiegcy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gjgqtujvb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gcpgchbox.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gtdrgncol.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gauqvzpxs.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/goukbjuke.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gpqjarowt.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gsmulhmaf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/ggdfbucse.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/giofmnxxw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gibfochck.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gguqnpzcj.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gqalotkhe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/georfnora.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gnqdeqsoi.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/goibpijfm.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gcmqwgwxs.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gqnnkgmod.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/grjwgpyee.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gtevoqzmc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gvajgklcq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gupcsmmqj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gvskqjsku.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gwpvsrtfh.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gdzhpbsnc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/guzapbyes.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gajfyjqvb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gqoiwkeyy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/galaxdqei.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gequbauvn.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gscuktwki.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gichrzegs.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gllvtgqfz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gsqzhuozf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gogvtxvlc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gqngqypze.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gamivfffs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfeuvywhi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/golojuhys.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gahvhrdfr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggicxrspm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gsmxnwtpq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gaifgbjwu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gloazjiod.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gvnhmgwbv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gaaptwiuw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gonzbndjy.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gvewmnriw.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gdvjabjql.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gjdxykstr.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gngsswxgf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gaiugcveb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gpmfpgxyg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ganqkgsym.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gkroqqdkx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/ggcpjvscv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gctbrdwpx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gwqsybsck.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gjioxsfyv.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gpodxdmti.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gsnurqgsd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gnpitjnui.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/guioopcxz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gxewasati.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gsjwrjsik.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gqhgmitsu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ghpgmlzke.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gnqnwjthv.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gxjpsabjs.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gfeblnxuv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gjmmdkydt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gefisuzqf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gkhxvrika.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gxpjvzxhq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gzhmlumff.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gzsrbdaiw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gisbufufl.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gxqbxxdwm.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gitaudrgb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxgwpwhpa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/goslffivj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ghrkssnmd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gfwqhykar.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/geguosagk.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/goulyxeby.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gekfwhckt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gqoyeuslt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gopwhyhju.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gjkbtphga.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gxjkyhips.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/grcngufha.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gqehfaxfm.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gymeahugt.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gghxndzvz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/geuubftue.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gwzdeqtic.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/ghnwaofnb.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gtresqauo.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpqgmajzr.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ggqauofvw.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggvpbiyjf.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gxfkvdhik.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gwqqusobx.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtrhbtwfb.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gjartdwqh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gggjkgpec.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxcerptdb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gugudnvvv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gdupckemp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gnououpcq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gqflfqrvh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gtonhvmdz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gkhpnjpyq.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/glbmwdmkr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gxjicedkr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gxnctzbwe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gkrkqmzzi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gevhinrhk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gzjftqcaw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gfvgpxazz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gptspamcp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gaokuayhl.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gobqvrugz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gdgzutdbj.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/grawhhszm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gpyxuzinj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gazznypfj.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gogcbnzzz.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/grbydfeul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gzkmzowap.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gasmccqce.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/geehbchha.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gpsnjxkrn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/glpuyrgdg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gjxozjizo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvvmspwtn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gybtowtae.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gpinfrylc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gdizzgvmk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gfeywwbtk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggsiicwwt.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gbmeuahsr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gupvuogtr.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gfdaryths.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gngveqboy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gxqmjxpgt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gupxgqefy.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gxtdpalyo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gzfqaputs.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gxisrmcfb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gsdvvhoqg.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gqjmjueqe.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/ggnlbgspa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gfdxorkwm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gkezqqpih.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzdogfdof.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gxwfhumti.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/griqrysri.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gqbqjbynb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gkutnycor.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gksugjnjb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gtrxepnzw.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gryegfyaw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gdkmvdmzv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gqkxwlwxc.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gibwaywqx.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gcflhooir.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gbbdvobml.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gjxkazjxb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gawttjuji.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gujndxtds.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/glpjmlzss.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gvmapdrnw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gtzdjgkll.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gvlzbefbm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gdyjqxvuf.sHtML


<!-- 参考信息 -->