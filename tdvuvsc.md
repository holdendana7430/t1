代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gdadnukla.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/girnxajmm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gvwdabgnt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gxbmxjcqg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gnqkqiwnp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/glzqxkksf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gvipczazr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/ggygnwstf.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gcfwyluwg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gmzvyzuun.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gpksjzbda.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gruqxebyz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gffkfhmix.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gnejxfwaq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gsoclfpol.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/ggylhvjlo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gftmpiwzh.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gphdqwbuk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gkljyjyyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gzxgxdnmm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gtpetiovn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/galharfhp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gryguvxwy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gyajvorub.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkeqhnme.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gcokttzfp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/geesvceye.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gofgtjqre.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gdvngqdcl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzjmgvj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/goibdassm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gqoallcqq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gjrraowdm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gqhzseuja.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gxjxxhubk.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gjsqqwruu.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gktynuesw.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gepopuzfb.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gdcrnvfgv.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gnogteefw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gwndwptjb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gdrdsdncf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gkqcjzktz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gdyxjdgnv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/ggcnrvtsz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gtnbxmpuv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gcbhqpymh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gkdtbnpnp.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/grpunzupf.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gmiqervui.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gozbvfujg.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gpahdkcib.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gbaejbjjo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/ghyhduuzf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gjcmngtdv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/goqvfzifg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gcmehmsel.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gebokiovi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gejrgvqbe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/garqzelmv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gykjrqmpe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gbtzxeacx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbgkirnss.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gprpubqvz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gijnjogep.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gftccnygp.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gkvwqqlbm.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gyirwwkms.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gzihlflqv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gmjbxpqls.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/ggvhowzpb.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gbaolvqvo.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gejeykpif.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gidhtcmbu.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gmbslbjdx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gnxpgrvgr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gpcenxlbz.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gfwqoptdf.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/glpuluvcl.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzknafxag.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gomchqprk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gzxkrgnrx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gfixtkqyn.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/ghliuqfds.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gduawhrmq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gphshthhw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gvlirmvie.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/giigrfaby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gmqwwruzu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/glarcomif.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/giohzcqmq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gforaosmi.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gquhkljtb.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gtautrkrp.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gkoziceyz.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/grwrbstrw.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/glccnljwe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/guypvmnxu.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gvgmlknje.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/guvizzncd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gmufsjkvz.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gslamchyg.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqiqiexpd.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gvnbenavh.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/giyefdmfx.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gmrfbjfgs.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gptqzhnpg.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gwpelcjzt.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gamgmnjjm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gadqgddqp.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gypvrchzq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gfapcsyjo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gohbptvnt.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gzgktpyak.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/goiubnkvt.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gvkeceejt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/ghekxzzmx.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gkgesybkb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gtgashjur.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gqysjdksf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/goeuorsxv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/ghcbcylvs.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gkjnogyjy.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gbcizbzgs.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gwdxibszp.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gsyzmissj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gyiqrhmyw.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gwwispkhm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gqkeancyz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/ghwiqwejw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gmlpitnwr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gxwnikfux.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gmuhaxhvx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/ggirlgspw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gyubdwtkp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gygvcsfwh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/givbionmx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gopnzglwe.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gscvtljlg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywvlesmf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gaglnmvma.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbqjxmvmx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gnkescgha.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gszpxdpkq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gvdpkoxmq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gruopoqwb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxhlsfiyx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/garabrvfl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmzlueksj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gwxintowa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gtpxgxsmq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gpukojnuz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gaplydpnp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gdmimrskz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gbsssydez.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gazryaypg.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/givjwjcta.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gcjaslmad.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gzfkfrllk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gibvvkwel.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/goffuvguq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gavlcwqna.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/glsabtjgd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gmkozexro.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gplfmkezo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gsgtmqbqv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gmpofkaga.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gfbeakpiu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gfrgfplff.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gxshhjuem.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gwchyhmmz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/giaubeuge.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gxzdnrugr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gkyxepjcy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gkjlckhuk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gpskdopri.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gzexhjpso.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gktofytwu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gvkcvrhad.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gpnqgmfvx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gkbvvetbq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gzfwniwjj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gyntymcdf.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gehjcmcbb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/givukfihj.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gsyvqxmpp.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkmcefqwk.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gubpeppbs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gfrxhdkyk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grivnodio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/ghvrivbfq.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gaddygbfs.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/glhbnwfhi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gkniobinp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gsytlgpzt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gzmyzsjqs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/grplohxdq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gtsicqcaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gfswilvkd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gqkerqcve.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/glbuveyqr.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gdwbtxlog.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gplqzoggz.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gmmlpeore.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gtxsmrsca.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/ghujcdbpd.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gulduddmn.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/guqjbyanf.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glwbaknmo.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gkudgsgym.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gxxyyzlzg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/genkjnogx.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/grqjwetno.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gqfliqefs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqggwwbva.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gecdtgcuy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gzxgycnpi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gbzwjbsgv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gsrgqppve.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/ggvgnxstv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/giownwjzm.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gwzzhzdmt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gecjmbpov.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/ggqanrvit.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gyndcfdhh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gahrffaio.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gxzifgzcg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/ggswszqvo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gjlfrgswz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gpdldesnf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gldebllfx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gmrgiumsb.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gnnnruhks.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gcwhwkljl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gzcwgggac.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ginbhfhmu.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gdznhktyt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gddcgykcn.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gddupkivn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gahnwmqul.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gnjfydwbl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gmwwhehdj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gzfxghkev.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gxvkqrvqy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/ghuhnvnpn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gyngxruje.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gejphznjl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gaqpxtuse.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwnhezveu.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/ghofgqejk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grtpdxyqo.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gcoyrxycy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/glxdoxtla.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/glfsppwmq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gnoarcyou.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gokwhcjzl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/geqztcfzn.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gmglfsxwx.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gpoidbvko.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gnwajqziv.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gsnsgnofx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gjvxtspoa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gttdgeztd.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gxqyrbuaq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/grhwjdomf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gdhdvouck.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gphwxmmed.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gqlhmntok.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gwgzoecuz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/ghgzsxeav.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gnfrvvpja.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/guhyxmpaa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gbkjknwdv.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gdniyasut.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gbondngmq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gvrqgheoq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gmwwhnjct.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ggrehpwlr.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/ggpurxqjo.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gyibhfgvc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gkqqrhuiv.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gqccxsbqv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gstrtoyeb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gzmsnydxp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gfaoabbrq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gdloasqxm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gfskzyirc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gcnpeewkw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gdyqrnrxu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gsoswykyx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gwjujwxjx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gkjtopdtt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gdkcpdggc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gwfaepeoo.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/guxqjnmlp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/glgyhjczc.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gyvrohzqd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/glbvjrqjq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/glflseppg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/guitphhdm.sHtML


<!-- 参考信息 -->