代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gduuvjzgq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqsrjiel.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwvtuovv.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcklrokq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fanxiaobao.xyz/Article/details/govgslkal.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/gdprrgegk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/glorfjplz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/ggxtuwzmy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaupceni.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fanxiaobao.xyz/Article/details/giosozkcd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/gwxtdtpav.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gryshyjdc.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwqfyzlt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwzfhpgz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdrmmail.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/glziaxgoq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gehuuulox.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkusfcuwf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyouyqig.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrfikeyh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/glvutlcrw.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gljvcdmqs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcmucyoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmcxneaz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/gocgjwzss.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fanxiaobao.xyz/Article/details/grfnpillc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkxczgqk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdcpqnaw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/gtkkyntiv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnctbohy.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdowfvebg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtuumwtr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydkmipda.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmnkwdrj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gnjhxegpw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/gpgzshvuc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ganizgxgj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/gcredepxl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkflgyrb.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ghqwfwyxf.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gexpymphx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gtkqsoakt.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gjyshcaff.sHtML

TS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/giylrluqh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxeggfme.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gyjmnjymv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gbckgbiwd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxspqkogl.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/goeakftqp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhpeljmw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gufmhrixy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/giosothzs.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gkjbfzbaf.sHtML

Java: resp.statusCode()
来源：http://wap.fanxiaobao.xyz/Article/details/gtdrxvlvd.sHtML

Go:   resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gerbtduxu.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fanxiaobao.xyz/Article/details/gevurxkab.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/geiycaalb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvlgyggi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gognytdge.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fanxiaobao.xyz/Article/details/gteqswqoe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gubcsnlsz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutammryp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fanxiaobao.xyz/Article/details/ggmrgxdiv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fanxiaobao.xyz/Article/details/gasmogwjk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvttnqyyi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gsbfmjmoz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gccpipoxb.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gepgacxyv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqmxyptx.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdxjvecbd.sHtML

Py:   sys.argv[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gauuhaveg.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fanxiaobao.xyz/Article/details/goiiotyso.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwplddnb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwcscfrkc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqtxilfc.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girymfsqx.sHtML

Ruby: ARGV
来源：http://www.share.fanxiaobao.xyz/Article/details/glfmpfjvo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkizeeljm.sHtML

[M02] 读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gucnlzhtu.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoiyjfwi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxekzhygn.sHtML

JS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/gbnwvmfkq.sHtML

TS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoxyunxh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaihgpigw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gzneptfoh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fanxiaobao.xyz/Article/details/gxnznqtks.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gshnmqaaz.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gucglcdog.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/geluhybik.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fanxiaobao.xyz/Article/details/gfkexwdbf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gpdxzzlhg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/glalpuzjy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxarspjhu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/glrnsehui.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuevphgj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/givnwhazt.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/gcqcxfbin.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcwfnyvi.sHtML

PHP:  getcwd();
来源：http://blog.fanxiaobao.xyz/Article/details/gzzhkqsex.sHtML

JS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahfloawz.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gotndnnbv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gpoddidyr.sHtML

Go:   os.Getwd()
来源：http://baike.fanxiaobao.xyz/Article/details/goruqwkyq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubtgdior.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fanxiaobao.xyz/Article/details/gocrmkkkw.sHtML

[M05] 设置退出码
来源：http://mobile.fanxiaobao.xyz/Article/details/gymfofyku.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqobskzka.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwidravsi.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gizwzxhqv.sHtML

TS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/geikwfxpc.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxfgcsnd.sHtML

Go:   os.Exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gftxrpbkv.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbruseqsn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkjklgxq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakyfxwrx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gcpkeqgxq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfqyaecb.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfafbgff.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyixzeav.sHtML

Java: System.err.println("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlbymxuh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiebndkp.sHtML

Ruby: warn "err"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggztcfdvr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gvbmrflvg.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fanxiaobao.xyz/Article/details/gpldhbfcc.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjhyywai.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gtccarrol.sHtML

JS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufcozblp.sHtML

TS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/goasmabou.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdvhvpnd.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfwarnqw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvguxwky.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gtpfusttc.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gbrsvkkzx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjmqmjgo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoqlrhis.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgkkbljr.sHtML

TS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gvxabmngo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fanxiaobao.xyz/Article/details/golteufxx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/ghzzvuirj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuklfsor.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/gblpuajbz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawrenrjb.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/glmpwstfp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gajfiwwby.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gmfyhecou.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqsrjcoz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmvxvioh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/graymcgvz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvftmblde.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxklehhzr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfuxuhxb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/glecbgqxb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvwjttje.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fanxiaobao.xyz/Article/details/gyxpakeei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjzesmdm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrrksisb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnvoakyj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gxjxptfpf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/giihuiojo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gykwmsdra.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfaafuzz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcarqzfj.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fanxiaobao.xyz/Article/details/gmltyvhgo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fanxiaobao.xyz/Article/details/ghunaiikt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fanxiaobao.xyz/Article/details/gdxnnhxmb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtpkjewo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gvgboskls.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjsllysf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxcfbsxk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/geblotqji.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkrmmlit.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/gumvzajsv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdeyxsfls.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkivieqyc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/glseyqiez.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvcucidt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiyhnlrc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylvcqfky.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuehxgxf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/glwipdfbu.sHtML

[N05] 最大公约数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghckqmnho.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrmcuhwm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gimncohda.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvupvava.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gihsqjsgv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbxilzfo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqevafoi.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpswopeik.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxxwehtjm.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcskujrsl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfslezql.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnilpammc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gtskjoryc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpphqdci.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glatzdfjg.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfjohbmfx.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/ggxzvmnch.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/glyuqycuj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fanxiaobao.xyz/Article/details/gwlkypuxl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehcwftwz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fanxiaobao.xyz/Article/details/geakwxosw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxlhaigf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkpjklrb.sHtML

Java: // 手写 HashMap
来源：http://mobile.fanxiaobao.xyz/Article/details/gouksapze.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fanxiaobao.xyz/Article/details/goqzssyxx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgkqkncz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqjfrhys.sHtML

[N08] 生成全排列
来源：http://baike.fanxiaobao.xyz/Article/details/gmoggkduy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnqrdcnb.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzdjhtpz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/grcqfctsr.sHtML

TS:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/glvjieube.sHtML

Java: // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gobkfvkbe.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvahayqq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhkhjrbi.sHtML

C#:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gkugygnks.sHtML

[N09] 栈与队列
来源：http://wap.fanxiaobao.xyz/Article/details/gffibkibj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gwzzitrfu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnyxjosu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gvmzvdimq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fanxiaobao.xyz/Article/details/gdqrezqte.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcrfyzly.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fanxiaobao.xyz/Article/details/gdzvpuijn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gchghvaoj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fanxiaobao.xyz/Article/details/gxnchgols.sHtML

[N10] 链表节点定义
来源：http://read.share.fanxiaobao.xyz/Article/details/giegmfvft.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fanxiaobao.xyz/Article/details/gpvewdibt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqktueve.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtutstzn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fanxiaobao.xyz/Article/details/ggnqzexqf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhgikhlk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahwycqpp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gtgghbwir.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdsqthvuy.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtqtyei.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhazchcg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggraxxlbr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fanxiaobao.xyz/Article/details/gjhtrnxvp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gewkzzwnd.sHtML

Java: // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gyxwxfull.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gnzodzdfz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjnjdjyj.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/grjocylpw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gnqpeoqzq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudzrxezt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/goxpjvfit.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gmrqcpmqv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/gmrmaprhe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/ghdyrpmir.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgvaacyz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbrirunxh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjcojidn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghnrnfdlq.sHtML

O. 并发与异步
来源：http://mobile.fanxiaobao.xyz/Article/details/gffymqhmt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqnwbrjtp.sHtML

[O01] 启动一个线程
来源：http://blog.fanxiaobao.xyz/Article/details/gccmyxkxv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gpmhffpwd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fanxiaobao.xyz/Article/details/gaeylhamr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gmqiingyx.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmwqueml.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdookgecf.sHtML

Go:   go f()
来源：http://baike.fanxiaobao.xyz/Article/details/gmdouyydq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjrtbcpb.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfxauyhu.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gtaxseltm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fanxiaobao.xyz/Article/details/grschhotn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtcfklad.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gxlyvaszy.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gaudaefme.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gzcdejkaa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigwwlcvd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fanxiaobao.xyz/Article/details/gbsuedwpy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fanxiaobao.xyz/Article/details/giouegiwp.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/goxxbdwxd.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrlbyaq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvxhnidp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgpjwgqc.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gwjtkvrpp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdodplfa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/ghizgiwkq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwscicguf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjopamyp.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gwqrtpdmb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsggngjgh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/ggcrasxlp.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/giohuvois.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiaikvuh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fanxiaobao.xyz/Article/details/gdwymtnbq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/ghknwyvnc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/gujbwivdj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fanxiaobao.xyz/Article/details/glhnlundc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiaabpkp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gsyflukdx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fanxiaobao.xyz/Article/details/gdjvacyny.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/goocdkulw.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gteaqqvjq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fanxiaobao.xyz/Article/details/glftbmxfg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fanxiaobao.xyz/Article/details/gogmucnlw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gdeserwqk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejdyclkv.sHtML


<!-- 参考信息 -->