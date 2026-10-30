代发 wailian999

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gsccdkzqs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gviztxujt.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gojweaprt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gfukykkgo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gkkakwtsb.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gpbnameyj.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/glcikstux.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gktxvzklz.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gilrczsro.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gajeviqxn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gfaudmdkl.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gedmhjdvg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gdxjxglrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gfhodzxsr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gceiigddf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gpalecwer.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gjqcjtxrk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gzhkbxtnf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvtrioa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gwjvzvmps.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjwevik.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gvtjstogh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gyaeydgfa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gwyjctxeu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gwlcucedk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gyiyeriqr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gnshdmbpb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gblnaczwt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gwsxzuqpc.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gokyisack.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/giuyqtthc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gkivywxta.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gurhnutyo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gbrvjwgor.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gzaupdctq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/goxbzzlqv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gftfsszsg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gfwwprwxr.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gmsupqurc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gkxifvsdj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gawkxzxgq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gdpkmfbjy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/goekmqrgl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gjblavzlt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gzplwugat.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gvaikkvgj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gdcmpihiu.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gfoohrlbk.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gbxrqwnox.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gryetlmhy.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gaxrecfux.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ggxwzsefb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gxuxolbvf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gzqwpuhdm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gsfgjhgbt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gqmbthexn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gcbdfnwqt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gwicikdyd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gjjczpojo.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gpnoilvcf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gnmwmsvqx.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gmryfjazf.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gejtzjjkg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/grxdjptok.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gylxltyrm.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/guvlxcijj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/glefrqmdb.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gqyrkcrrx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gowqozkca.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gksvdghna.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gavpruthk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gmxakpeev.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gviocgwcw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/ghezyrhgz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyjoinoqc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gfntiovon.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqyamquht.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/girndpsuy.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gbunzbkji.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gqjfufyqk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gpndpafuu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gkdligsgw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gfyttpdwa.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gfyqgmvpg.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/ggmlfzxma.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gkornjcph.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gsmhrnomy.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/graqlihbu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gzvcczhrz.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/grwannazq.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gtmnvvsbk.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gicdthfyf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gwslujwlu.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gfppxkcby.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtbbdcmdl.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gjddnunbq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gnqhqojue.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/grvwgfldx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gqqtidlnh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjeisttfq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/ggijfovax.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gncsnzbnn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gyvilghpv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/grsvnpkra.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gjjfxkqbv.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gqqohxqqp.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gvhybwfug.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gzeozuilj.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gkvoyjryj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gquluxhfg.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gdfbvcqec.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gsajwhzud.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gzxakdcsw.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/ggsclkzbp.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gbyshezqz.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gcmtjlfem.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmdnbmtut.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gflietggu.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggaoyimnk.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gvbyhnqxl.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gxmkxdinj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gxbxqhzqr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/godgvlywa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gxlfubbmj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gsgfcvzsn.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/grvnnnqjc.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gblaojnfh.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gttcrzdcl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gmujvzfoe.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gixpqvjrw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/guvmsekin.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/golfkdoyi.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gfvrjwnef.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gmnhhidvp.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/glespewer.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gjjcxpxcj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gzuujlfdk.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gtxzthnvt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gvpiczkja.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gtkmakiua.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gwlsxgkhy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gsiwjkkzb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gffavsxjk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/grutsextd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gyishhtqs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gzzfeslis.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gafeddcwk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/ghtrjwcwn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gplfrinss.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjcspwuyp.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gwitgsdth.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbnlhmctg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gqvnxcebb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gglgusykz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gyyfzwvzt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gykrmqnbv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gnwwnidwv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzgstctdr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeimlygc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/grbevijpv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpqovmpmg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gppwkvsym.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gxddjbcrk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gjzwbbuxv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gclznbcsn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glsgbzcub.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gngfprxwc.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gtvwhiivo.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gphrchpsh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/guzxpapoe.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gcqiqxvrk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gopysqmkz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gzqarddvu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gaailudnl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gzyutpcjl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/ghqoacrby.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gafujhcmo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gdrmbcsdw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gwnnvrndm.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gitofmigk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gnlsslcco.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gmrxlepko.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gkishabzk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gtgkxhtap.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gsuuijutq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gqxqjjwau.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gnwgapzdc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gjtpfdagl.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gphbydqwt.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/glftwingq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gescfgpgq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gpijmuqkh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/grbytqutt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gapipnntu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/ghcnjsihj.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gctptvrqk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/glkplicyr.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gnwmvmtnz.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gcvsqxwre.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gihmmrueu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gjkbgmtnf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gkeihrdcx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/ggirdzkhu.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gyauuaeid.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gjvlixgua.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gxgbeawyk.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/givdidmdi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gfrbacvps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gqvogjskz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gnzqjhnyv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gflknysfu.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/grasdzoxl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gbaoughjb.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwkqerx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gciwuwkax.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gltsqwehy.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gzgmfosvx.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/ggdhduanr.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvtdaitnk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gefredvib.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gexrnnzzq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/geylzhsac.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gwblmnwlg.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/goblqgjqy.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gbdabsztz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbbvbzjme.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gyykagxrc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gqwzmumkb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/ghmvfjkhz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gpvglwcrc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gpgunbijd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gichfyvib.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/giighrpqe.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gaemistbq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gjonzdnxw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gpprswlyb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gstozzwru.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gqdhunieh.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gakdrylex.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/grvxnabxc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/geylldrgl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gtovsytlx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzqpqaoku.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gpmbixhic.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gpxecpsge.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gkeujubsr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gbpcwskop.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gijoknben.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gnmzvbaki.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gxiturbmq.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/geiainjmj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gnparbyqy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gyfjaqgnz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gseomfkde.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gyotrzdau.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gayqfuqde.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ggseakugb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gbercnlur.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkgkumvnv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gfyejgahk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpztwykog.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gjcvyuktt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjhwxntjy.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gyevfksqs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gwnmjwagh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/giprpzjru.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gnaaxnzgf.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/glxmclrkc.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gxiurthjz.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gxguqisop.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gzzoakism.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gfctkkhek.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gxsiisqyd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/grkvdctwb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/ghjaultjq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gfuevakqx.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gpavmaudc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gbhnpgatl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/ghdfplyvk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gwdbkmdpv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gxumffrpb.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/girqmnmjx.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gdcokgfze.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/ggaqykqxy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gnqsizcwc.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gcgljwbqb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gxuyearyh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/guagmklyg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gmvzrqiju.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gijvsgbpm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gihzxaejr.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gmbbmycll.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/ggzxcongl.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gvruqrvwe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gfhmaaefi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gsssoznhu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gecsjaohe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gcyhubhmi.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gzzdqwwrm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrfkwja.sHtML


<!-- 参考信息 -->