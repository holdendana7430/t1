代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gaamscwqp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/geibqodif.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gmmoznccx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gfirdvigx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gxybscfsi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gqiykwffh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gxudiqmpl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gleesmqyg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gquxwtxbo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gcbmlnjui.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gdejfowsg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/ggjekolwd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gysgymkev.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gojvsxisn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gvbjdirib.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gswezjjzg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gjbowplma.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gshlpvyrf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/ghabkcens.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gwpzrcsli.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gmsmtkhvz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gamihhjdv.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gpvztuwdc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gijhzgtcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gtlmeskvu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/grytqzusm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gdxwcfzrp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gzheboxem.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/guolmpgge.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzygqgjdz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/ggemfmxmg.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gscrdkyjh.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gtyjgplki.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gxeclnjab.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/ghafrtwwf.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gsmbplcsl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gicpbcprh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/golizeftf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gmjurhgtr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gcbnsrmpm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gcmmcmnsw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/ghhbupoye.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gfkiyocnv.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gqvqdikdt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gozrmroxy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gorclkozy.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gthpnxwlj.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/guzqexygw.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gjlxkezgu.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/ghitjcexu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gxvwabvxr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gixzgtajt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gscfbdglo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gezaestxz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gbjxnqaor.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/ghkcewskt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gmscnkzld.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gbucbmcnu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxolszkup.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gytdttfut.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glhjzonhz.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gdrnenufu.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gdorrofbd.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gmxdavjpv.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/guhseuzjq.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gikjtygee.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/ghdrcwcsl.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gmrwvsxtu.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/grgoqkdhu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gpindjxjv.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gnyyflvdf.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gtazokkyq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gzvjfxuaf.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gniqueevx.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gsmheaogz.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gpkfcread.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gujfuftes.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gtlvpefrm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gmifwlukb.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gihyxpkqr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/grckiystr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gxxeexdgu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gnwuryoax.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/ghprrliqh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gvtigoudq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gnmteziqx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gvihnepje.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gznrwcdoz.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gewvnkudd.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gwsplzlap.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gebezlgwx.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/goppbcvcr.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gwxmpdvxa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gkyheyrxc.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gombvpjlq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gwlghnxkc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gisccrmhx.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/ghvdqwbiw.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxebnbmwu.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gxunlfvnj.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/grgfawuzl.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkytwjeha.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbjcqaery.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gayfjnqez.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gthuerocg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/ggurwocgd.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gjohjuike.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/grbkppyja.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gvceksksi.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gkvtzfgan.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gwtktjkip.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gddjhehsq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/glzqjndkf.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gpdtcckgc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gdhemsqdw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gngtinvov.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gdcizhadr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gzjknlltx.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gmeeaawqq.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/giwunfzrq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gknaghhui.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gzrlvboht.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gnhrajivm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/glyvyfniy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gmkhlkfau.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/ghjjogbdq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gejvjdkto.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gtfelurga.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/goiisfspo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gjbsrvfrw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gxbmcbwys.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/ghaxqubzw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gqpoeorfc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggevrrlqj.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/grzhjmgrp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnwnmskqj.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gjfxaylju.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gszxofbuz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gljfjxoee.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gdpiedxjr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gkkdkbqeh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gafnvngvi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtfwauebu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gyfryrypg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glvtuxdvs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhrnmxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gfucivxiy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gksblmabh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzqygqkyv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/grivkddfe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gwctwmhsi.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gvbuinwar.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gufhogstd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gvqwnjhkb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gdkvtvzgd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gwobupztt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/ghynymchd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/grtgsapzo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/glfhtauqq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gmcjgdnuz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gydoehtjl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gnhzsgpwn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gmikxxcvd.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/galhjwcud.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gopdphxlz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gizpwpxmn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghugujlsa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ghhvnbugv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gdeyjdppx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gzokozehe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gwhnmmnzp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gngzpxgob.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gidxtkitj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gybqkpyil.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gnoyioclr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ggeneqjum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gdbotvwrp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gtbvrqfnt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/glzzafzav.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gokcilqeo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gzooeymqq.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gzjkzeqbc.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gsbagmrwl.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gdbmknlww.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gbjepfume.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gaxtqnpdj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gktynwguh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gibrxpyxl.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gzdhqautv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gkplwtfxg.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gyysrwjgb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gwffgspxy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/govsajpud.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gaqknvosx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gpsojgwbn.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/givtgcsua.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gmkuurvjd.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gbeijdomz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gektudopj.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gscueojwl.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gpylnzjmz.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/goyvrcnbl.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/guufgecku.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbrxlwpke.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gwyeuonde.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjiodureg.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gwgmjjjtg.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/guklvsrwn.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gyqvokwqy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gkjrpctuk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gdzplhyrb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gpewxnnhk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gkfrhdoxi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqhrsclmn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gcddbxxdb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gqttxqpvz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/goclbnmkj.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gbztlwsyx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gvwmlaucl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gjjfpdzxj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gjpvghftm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gghnzauyt.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gkioxwmlt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gsrxdzwwg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/giyqnszzb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gqpjgslrs.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gsfaxkbbw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gwkoprtes.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gidvuwtzv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gzvuptefh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gptlzzfhh.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gocjpesdp.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gxgtiquja.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gnzoszobr.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gwednlxcd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gjladgmmp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/grpdsallv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gnfstchkc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gowsnkpik.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gxwebhjyx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/genmljjsx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/goydaxtkz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/glsydecbf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gcewyekyh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gunvznhbx.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gulmxicfo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfmpkxalz.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gcbwzwdvl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gkhjokmku.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gzycqczgj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gvqxbwxjc.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ghldowlvj.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gmwyvlofs.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gzvscdkph.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/geykthyhn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gniblmoqj.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gkwrawvet.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/ghqlkfhaq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gwaqjoqwh.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gtekydqrx.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gplrkqajb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gygzzsvfj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gptndklll.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gdcalqynh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gzyoglfjp.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gqnyoaofs.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gzdvcmnep.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gqrroqvsj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gfwozkxox.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gfduwhvxb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gjkedjgza.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gwutesnkd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gbnfldscg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gnhtaxzoj.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gbkrmstes.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/grqsfxhft.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gqwqitqhx.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyazxnjy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gejglzzzh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gzcnncnse.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gimwrsant.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gyibivowp.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gjwoyhfpl.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gmemcpczj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/ggrdrbluy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gjjyctmsk.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/guzsutueb.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/guaghgomz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/ggiqolxxa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gzjrqmfwc.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gjxavcjiv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gphthowjz.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gtoqebdqc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/guybaeuwc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gqvdqrigr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gapylwfux.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gutptjxlm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/glghwsccr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gezpxjbrz.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gplledkyq.sHtML


<!-- 参考信息 -->