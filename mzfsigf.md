代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/glsvzujjh.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gcudqqkqm.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/giryyqwls.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/ggwsiosbh.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gullfudvb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gjnrekstf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/ggeppejqs.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gpvrlmqub.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gqgbvutqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gbnkesyra.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gnilyqotj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/ggczgzfwt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gwnbjvhzb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gazigjute.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/grhtudhht.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gztccewrz.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gwttitlku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gytdrwxpp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gaezqygfh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gjtohntfs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gsmbnvhtv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gxwhjpkuk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gkmwcdnzk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ghbkmbasm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gemxjhvgn.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/ggolumzkm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gfhkmwqqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gigunwtto.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gdeegkywd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/ggowcxirc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gactvnumv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gugowrrjt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gfrfnnqaa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/ggvrfnlui.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gjdxpmnyq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gwebfqgfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/ghgdmxbbm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gqawolxis.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gwomkyngw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gihiyhpys.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gsfzbtgei.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gvnmiaoxr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gclavkypu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gjlhiapeh.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gdxrerxsy.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gdcesmaot.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gdsjfokzy.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gynoveztu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gfquyhbcb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gnbgfrpbf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gkzqldszg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gclronkqv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/glyxkarly.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gkvxiswau.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gzbmbefwf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gawxxpdwj.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gppiahtbv.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gstvqjlya.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gogemggcr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gozfhhttu.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gcrptckvx.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/ggjffazco.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gyqftogjq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gxdnkqzcb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/glnxeyzvj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gnfxqfkrv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gvtzejvhf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/grbbndtyf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gptgfhjza.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gfuszvenl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gouburdor.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gjoojbklp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gipfvtrhj.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gqctgrosk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gymamdyfe.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gzkrcldxt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gwuxugfhi.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gentpmjgn.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gsbxtqrht.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gmrilimxx.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gzvgiirhj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gjmiocgwl.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gzmirohxr.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gixcnbszk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gvyikqofx.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gxkqkzekp.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gossjgklw.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gquccftwr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gvzmnwfme.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gudprwgom.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gwcqspacp.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gxfpnzeob.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gyszkknrn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gwmpknqce.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/ghygqqqaz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gshorxjwr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/grlxznbbq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gohbppqyh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gquepcfjq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gktzyizjp.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/ggiwfdcox.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gngznoqnz.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gvcuwiywc.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ggczfunvh.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gnuyursqa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gyifdhdph.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gawymsevu.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gzryjpkgy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gqvitpadi.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gaolvqfxh.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gjtelsrfh.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gkbfmvyve.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gsyaqwqsh.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/grjqeanah.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gkgmxwfik.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gelbgswge.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/glsazayoa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gsygqpgub.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gmbterffx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gcavykaim.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gskjtqmiy.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gpixzwwki.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gimzaizen.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gooqonhve.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gdlqmmsfu.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gdsoivqco.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gicognhjb.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gnrmwofmr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gzqhjizel.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gpocmleyn.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gabmozvfs.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gexwtdrvs.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gqlsldhpr.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/ghtvwqhpl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gazjmdixt.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/ggzdjkcze.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gneasgtvu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gqvcdycsz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/giklibpjk.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gikomijcf.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzfqumemt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gmhmkahxx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gyjuarhgy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gwhdofnae.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gyzyfnbda.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjjdrflhc.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/grpbqnyyr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcftldfmc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gcvdcuvcf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gbyhtlkwg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gzfnevtsu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/giykeeieb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gstbqidsp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gpbnygzfz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gewxzjbia.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gjjkwxawo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/guzgtfwzg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gxyzvupky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gcgcnkgun.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gvwwfrpgt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gzfcpwmsz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdpcpeohr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gukubzozr.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gjfdsmifz.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/guxbdlodo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/glfjvlbgk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gokhvelsg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gnwuakcrh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gbwwhsdpe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gnfehwcit.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gsavfqyos.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gdlpibcpq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gwauucctb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/guabphobf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gbjxcfuoc.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gajhhiywn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqhfsvoyr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/guirokduu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gcqyfkouc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gasreobpj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gadphnerr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrepqhsp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gnqgpaiye.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gelvnbtau.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gestmgevq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gesxnjctw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gyjkzgnjo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gqgvvhygb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/godxivdwf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gjpnbbznu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gayylccxp.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/graweykkh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/grfbrdfku.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gvteehcdl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gbcuuujvu.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gdraptmjj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghthkepme.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gxzkueiwx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/grdwgpgri.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/ggnmegpfn.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gipewcxbn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gvfovtyuo.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gbityafxa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gkpgahjgs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gdpoiealp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gsgkqkggh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/glctiowgf.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gjwehmxdc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gdkqoewwj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gjjweoeag.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gkkxotbfw.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/glbqiryrl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gtqpefitl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/ghfmpcdvh.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gzenxpbzg.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gscijapoz.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkpaaesdf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfpplnioa.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gptcymcrc.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gaugfltyp.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gtcilcyxx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gtsekvhur.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gmjsnngfe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/guxgyxjye.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gttrpirjw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gfisfdgfu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gpxtczbkh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gcagtzeaq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gaqwtxvpt.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gscajucmf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gwbqdjicr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/graunjlxa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/genhfumbw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gvojgevfq.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gqatelaww.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gfbvpteqk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gcogblcbf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gypyreeoi.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/geirouxgj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gemosfxwv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/grkyvaovu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gicbdbmxa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/guimrdumm.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gslhilhqh.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gloswcgij.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/glvbnwmtl.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gvmjtogce.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gogiovhke.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gdtbeexjv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/glsxqzunu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gwanjlhgv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gpweleknl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gjdywkbho.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gvcioigqh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gphxoaiil.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gmmvalxyq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbsdbitkr.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gufivacjt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grcjyjvwb.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gayxkshdt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/ghqtrwtmd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gjsjkpgsl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gfwnpinyk.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gieaamish.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gfysbnogc.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gqjyejwsx.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/guxrmgpgm.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gdwilkjgr.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gwadulpdy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gmldwhzay.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gixtqwboi.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gwjabwqsk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gataanduy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gxmatlppn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gqgxehshx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gfghxtpkp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gyzlulrht.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gfvlllrbs.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gltuupgff.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/glrcyasos.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gfgedckqb.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gsbhqlnis.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gmmkmoyqy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gqrcflizs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gyjizggwh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gxxjfcfhv.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gsxnkmlmd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gbswycqao.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gepiefmor.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gchvdjulx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gbeeufvhc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gulmgtxba.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gcfmtkhbl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gwoqcuwcl.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gwriqwwvz.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gvqeqzgqn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gbvczwgzn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gawqgyzih.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/glifqabcu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gekjhiyvm.sHtML


<!-- 参考信息 -->