代发 wailian999

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/geagikrfx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gvrhdyctp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/ggnjrcazs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gytdnqyfe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/ggshhyyxp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gkavhrmkw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gqzrewgre.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gcdyqkhmq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gargrwcrv.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gsecpzowt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gdymfualu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/giuomympd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/glqmrdpzi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gjtvshxvp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gdztlhqeh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gpvpifxti.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gvogcyxwa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gmjkenwgw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gczdqzdek.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gwdhjwkrw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gbjqmjpoh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gfssraqfd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gogjjcmwo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gftzecxkb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gszkkjpsz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gryvevqtr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/goxdjinwt.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gpgldamzc.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gskcjeknk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gpljgqohl.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gepxdtfwh.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gqsmkndjn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gsuyztyyx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gdfgxnddl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gugyegwyv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/glcsersfh.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/guyxdorvq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gacadgezq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gkonmunsv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/ghzeezdtf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gvwdcqksc.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/ggkuayvck.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gwwebawtk.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gzawximlq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gdkptjlql.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gqzygykaj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/glidygczg.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gdpvtwlun.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gwhfwmhla.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gkhagrskv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gmptoscnx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/guknuhyap.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gzizzthsg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gskuswcrv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gchmuxgax.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gwoeccfvz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwlywyhoy.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gnuzbbctb.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gsynpgjyf.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/ghoxqmnkh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gligxohvb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gryhtsypr.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gvnkmlcng.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gilavsnyy.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gejgrmhhc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gzgrdwzdz.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gaxjfzzlp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gosxqfybz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gnvjccskc.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gsgsnhzlu.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ggnpxszix.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/guttrhslv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gviiayltz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gbtgrnewf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gejbabbfp.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gghpqvnwu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/guktvypzl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/ghofepkhj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/geidexmjm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gbwwuyakn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/giwbhzloj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gkjhmoosz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gsasbdxcl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/ggpzrxdnq.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gvdsqomdd.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/ggjeksibj.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/grppvckxa.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gmkbxfbqa.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gsoufzvxq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gbztnvkfn.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gvtamhzfl.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gnykdfpls.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gbvvbpxpw.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gvseqtjky.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gonfxfcfm.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/glrepoleu.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/givxwgehk.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjusfqiri.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghbzjvgnt.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gtsqtpzwg.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gvajoerrq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gpukmzgoy.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gpcxeaetx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gcbultypv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gsafhgbyu.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gacrfooae.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gkyfptosg.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gfngaguna.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gqemtnfak.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gvufwhcpy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/goyggocgc.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gecyycgew.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gyfbnrcip.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gingyjgrk.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gnbfzklos.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gtbkgmtnw.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gdhfifsaf.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gkeooxmlw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/ggunbcmib.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gezozmkew.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/grhyrezbc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/ggqwmqhuy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/geldnbpvv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/ggackduce.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/grwppxhcp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gbvwiluwq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gwszhrsbm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gmhefcdra.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gubftqihc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gunazroxk.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gxntpeldg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gasxrssqb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gqgryvjwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gxrdrxrxv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gkglzygpe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gpubqqknp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gtivkfgao.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ggwykjufq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxmqwynco.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/grstgfwoj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gfxmqtlbl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gridpeoof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gvzfpzugj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/guqgdpznd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gsxbrsqfj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gjnzgozeo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gzyfnxbka.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gvzdtjseu.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gnzcbgzes.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gnxaeetvp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gjvqvbxme.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gkmbssuuw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gvrepwnqi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gcyujrwgp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxfexjakv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxuzrrc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/glmpzjocc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gtmwcxpmu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gqglmegsw.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gqrqvikxc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gtkgutuzx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/grqjncdow.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/geancknxp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gjyncyxue.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqiohavdj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gzkkcgutc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gcafsvykq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/ghrkbafsh.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gzjcydjvf.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/grdnormdo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/golchchhx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/ggpxdwlrs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gteltzewz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gnvxbvjkp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gglmrhgpx.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gtubmettq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gndiajhgx.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gnlmjyjvk.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gbusdffhw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gsywxfyjv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gloabdzif.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gunmwxaxz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gnvswqrpa.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gijzutykw.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/ghmrafjrk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gulbugijf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gpvohypma.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gzhzdawvs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gxkhpmkoq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gbscwcdup.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gsybtdknq.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gomwgemgg.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/grynkhaod.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gyxtopzwj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gcnubhwyd.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gojkbthtu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gdllsiefl.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/guochhbez.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gluupynso.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gmufoyskf.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gseisshbs.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gjhugmhfb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gtgoevwzi.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpelxvaxe.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gbdfqabpc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/guajrcrlx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/guukpkmuw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbmqapdyy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/grpocoute.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gcxxdqdeg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gfauxlwfb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gwiviqayy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/giryjaojd.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gktfsxpng.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gcelaypao.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gxlyppbyp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gmmlnmfpi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gmlxqdfao.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/geydgkxpi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gjchgghoj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gcsbzmptf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/ghfpexglg.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gxpijelkg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gvbcnemyo.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/ggilzyhts.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gojvpbgza.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gubdudpzr.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gbjxajrqc.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gfyxhesgl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gsjjvfcab.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gosdkdlmw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/ghmiqkgxr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gnrjkacfx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gfbyotjjr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gbdqmvatu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/galofzryp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gjymedlwz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gmdnumfau.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/georkzzpl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gdsqxrbyf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvwvnflbv.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gbmfqfxqk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmcolmqgt.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gegiyiyei.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gjjsdwiji.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gesbpukss.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gnujlijla.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gmwjbbmyb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gbeeojprn.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gqlmpwndg.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gdsyjsirc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/grbzavbmy.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/ghfodrrqs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gzwhopidh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gttncfvdm.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gplwuqbap.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gtotghepa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gmcnwxpwd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gkgatbnsf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/ghavbfqzn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gflrajazz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/ghymvhcxp.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gepxkzbgw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gtaanyzlc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/grobokjgu.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gojmdlwpo.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gignmdphw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/geozgoizm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gerchkpqs.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gfkgiwmrw.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gfidgfmvn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/ghikkqigs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gfpktqosj.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/giijfmbuf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gxgcadgbl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/glpipswuw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gwavzffml.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/genzfpqvg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gqdqgxldb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gjcygmams.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/glzocxjkq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gejffejxt.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gnbwwckrn.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/govlrdlkm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gifemmsxp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/giabwfoyd.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gobputuhl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/ghhchhrrg.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gywgfwvjv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gftaldluq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gpogulkmd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/givjxqmgf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gktvhscxs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gfedbgbwe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gseuxqqcz.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gtnrppcls.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/ggdjlyfae.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gogitqpir.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/guulujfnv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gutguivpq.sHtML


<!-- 参考信息 -->