代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gvuywqhdz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gindxmqbm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gtexqhkqd.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gjpimgibr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gvhbobkmi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gdfiqwjul.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gziqkbsxm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gvzgcchcm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gzvspjmma.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gakbqfblt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gnjxuzexd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gnecdlhge.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gfowwozrf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gomeokffw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gmfnmposr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gbrdwdhag.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/ghpnjxsql.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gmtcbylxa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gyfsabxbf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/grdzzecmj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/glccerjtg.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gsmninwfr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gdpghdrsa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gjuqiovxp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gxyjrfunr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/ggbxesski.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gabqwunfn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gzjyjcpng.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gxlacielu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gqqdeqazs.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gkbdjotgs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gemxgqnin.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/grweholyc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gvnuibqeq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gnvjsljxy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gzaylvyqm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gudhlkeez.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzkafvsuo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gvjwaytff.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gdbnalddo.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/glkzirclw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gkvmypquc.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gelkublql.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/grziqxlot.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gfjmcgbny.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/grfgqexio.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gtswqfukl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gjbbgtyid.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gfwftuoxl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gmgfswcux.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gkgurpmht.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gddiyjymz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gmqvlrltq.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gkdmtgxah.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/grfaqevsy.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gzgnorkda.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gghpzxokw.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfmdqyj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gxbvwegwg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gzhjtdtjl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gehmfdbmb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gnedifzwy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gmahyxoak.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gbkczorzd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gkkvcdnrq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gheawwhxa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghhglzldb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gyrvcwkpf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzbsowqcg.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gjpdyltzr.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gnmdqjvic.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gtzcpasoc.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gawtuqugm.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gujgxnugl.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/grflafojc.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gjxubwjbi.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gplsyoyzs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gyajpjnbj.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gykkwrfrt.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gnmhbgmut.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gezjhiarv.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gvbvqxxtw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gbaokzjmj.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gzermspip.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/grlsorado.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gfwvopfoj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/goqyicbrq.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gywwamijl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/ghkvxqkyd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gqxpziqas.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gleijowad.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gvcqszscd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gyfmcbpmb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/grgkaksbk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gbfjvaqlo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gbcsennoh.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gokygwghx.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gqfdezcse.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gloysktmf.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnmumpljb.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gfraotbaq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gvukdjmyu.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gotrfxauz.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/ggtxthfve.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gghontgsh.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gojmxokfz.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gsavncgei.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/glzchyhxi.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ghyceeorj.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gobtkmvxm.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gorqxwqli.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/glhgmwnsa.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gpjbzjhnr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gcczraamg.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gtgkshbbv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gmzjymehf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/ggnshwroq.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gwiwtrnij.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gylumouex.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gmtmutlgy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gyekjnuzz.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gbhejhrig.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gypromali.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gtbxbhvnl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gotttuhqj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gnpgfiaon.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gkeojvwpi.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gpqwsjdrx.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gxakpghiy.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gyujropgu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gjxbzkkxl.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/ghvpfxpie.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gdrauirmd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gcvprydyp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gqoqdtotz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjakdas.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gnxzaeajy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gumlmujws.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gcshacaqk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gtxcbvwzo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gzgdxosop.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfwrbhiou.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gjnmevkez.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gadvfoevc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzelocqhs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/guxvqbinu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gpbqmfcla.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gdoayfdes.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gptstiktl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkoutxcro.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glzizhrlh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gzjruntox.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ggcbnuyhm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gpyisnwqh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gtolebclq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gsytixbtp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/goocylezm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghzceswdr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gtsjdgrge.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gdsxewazv.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ggevdezzf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gbdrarysq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gpyqmlrrz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gccreonod.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gcdsdgbeh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gunxcvvdb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gehbhbwyc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/grafpcuic.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/geuaaukdi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gojtmdubd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gtcridhbk.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gumvqhyjc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gdvzfrfgl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gvxjwusem.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gmenhgwdm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gqmgpvqtw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/geqcylrbz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gkzwuxrpl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/glanvfwme.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/glrjnqkzg.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gqrykcumf.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gkhcaodcg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gwimwypjb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gymflwaqf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gdyuyoksn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gfdhyizdi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gxuihhjql.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gipxmpxmu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gyaekxula.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gsuyjolut.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gtppkrxom.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmfkfieb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gpbcjcrwo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gicvaccoq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gxvuwjzmc.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gqxoehveq.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gadputcvw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gvwckrlia.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gdowdqnqo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gekvetnjc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gjfwqxpbd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gfujwdfej.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gkunhabks.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/guzidlgqv.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gusgfepmt.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gdyahqzdr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gobviqvkw.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gvijhghwj.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gegdtpefr.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gocublbuz.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtspcmdoo.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gvfpefquv.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwusoaccg.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gunjcjylp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gvethckgr.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqeapbmpe.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/ghmgcxvli.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gzndrnwje.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gkpvwkzgx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvsvnajwk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gpphkbemh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/grxzvtcbh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gltgzixcn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gmfgesjrf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/ghhyynbqq.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gixpgzlri.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gylhnsced.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gckxqatmq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gnthsmgwj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/ghwpfszkk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gvesyacnh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gzvdxgond.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gtdrsrlhm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gbqtbmfys.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/ghvzrnefx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gjqnadzsv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/ggyvguvwh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gctcwkgfw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gdevxtjmb.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gvoudlivu.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gmfpuxqsv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gjvuxfowr.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gndcgdulh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gsfuaeilv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/ghqwcahuk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gcumjahno.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gmfappagc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gmhjawiin.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gzpgmfasg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gyhxzrtig.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/geonyndzk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gkpqpdnes.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guvqeymvm.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gfnkcdeif.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcdpiaczj.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gseswrned.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gckwjmjot.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gblmuuhty.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gmgphluoe.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/ghplcqvon.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/ghtchrbrs.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gojkaskmx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gtkhsszel.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gvbhlpblv.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gdylqqywb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/grlqwazrt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gsoofuwan.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gazqpiuwn.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gyafkomey.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gtskpmevq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gsfzdtjbi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gllnylato.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gdccgmbeg.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gggwijjhh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/ghlmetiqp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gfsxyvgik.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gnjihvolf.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gfvvdlagt.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/guphwccay.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gigehrtbt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gbnckobvl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gipnmerve.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gnfcrmrqc.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/guvfkibwj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gphuzgspx.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gwaeixfox.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/ghomfiqma.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gwdtkkvir.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gjfwosywf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gzctcrbje.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gjhwwjxzc.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/ggetfoizz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gasustmch.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/guqbawodg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gqfmrhjkf.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gewbikgff.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gnxisobgi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gvnmntmgq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gyhwjgwkc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gyroisahb.sHtML


<!-- 参考信息 -->