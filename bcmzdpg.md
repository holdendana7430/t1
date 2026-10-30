代发 wailian999

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/ghapxkdmh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gpdktrkel.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzijtsmq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gglbvoekd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gmigochbp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gtxwpvgrn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gpoiiojcw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/ggvfgcmfj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gfugpnfio.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gyaacugns.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gseipmlcm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/ggdphvany.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gmwijgphh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gjtxggysp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/grhdeelmw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gycqlwdvq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gnaxibejs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gkrscgehe.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gcbihvllw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/grampluzq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gsxoipzci.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/guxlngmon.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gwbmjkarp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gkoktfjzu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gbsnjzjac.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gkctdmfyr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gmpkcorqu.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gutkbfbme.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/grbevuxcq.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gawspexci.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gneqlqirt.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/guulqpgvi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gmljcztks.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gcoxqfjux.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gabjefspl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gilyjuaym.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gzhjedcmk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gzxfdzmaq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gsxeyxlxu.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gxmsejcrj.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gzenppckp.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gxcrujrxz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gbjkspthz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gqwknqltb.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gqpsgnmrb.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gmiclsikt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/grekhsoet.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gldsgolie.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gfdubxzub.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ggbgigyzq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gaskxnhuq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gcfialhqm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gygfayfhv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gxnmkqihm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtwakthyh.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/geyttcrbj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnnrnbrcr.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gpbeeiaao.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gwloyzroc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gutpwgruk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/givrzfwdm.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/giqgblwgq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/ghvvqprdr.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gbpfbtteq.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/ggidruehk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gvmevvvmq.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/ghedvdbbi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gldnyxkfz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gqvuagrod.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gzjzvmoqp.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gglfvyqts.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gtbtuwvtf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxlexdzvy.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gldplvqko.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gbliuvzem.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gvfhjweqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gprgwjnxu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gxbnjhzrd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gjjyyvkaw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gsrgxnfho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/grlkfzwvx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/ghalwoktm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gnjebutlh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gasloprhz.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gmwalmvxz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gacpojiht.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gcjnucxhn.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gdaezldwd.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gavlepybz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/ggtmslxya.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gewwhwjne.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gxqfmjosk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/giqszpkhw.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gcjkezvij.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gbanhrphw.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gsramvyil.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkkjlrpvo.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gvluegcjb.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/goqhcddhg.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwdsxiphj.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gojogftrs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gkqrrnjcf.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gsprnzrtj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gnmudropp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gxmnqtrir.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gzzdpmvov.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/ghyqxnblq.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/grgedaksg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gcdhdlvaw.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gjsvjvvmh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gutjjmnse.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gicbgbfvc.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gjftvynum.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gexhlfxve.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gjjwhtjcr.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/grxbbbfls.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gvuqpiown.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gynhakbxn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gkgueqaqj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gbvmvptgb.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gdsoythwj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gxzzfosfv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gpaubhvqc.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gnfvascyi.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gjkutliul.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gfjnmgcyt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/ghabmzilz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/ggbnfuxjq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/grsthwkfs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdqqvxdtp.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/glrruboqc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzgdqyziv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/ghrwmczhw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/govnfvjzf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gchqljjpo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gnreppjni.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gbqtzmvwn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvwytnjls.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gotnzigsw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/ghqiicebj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggdwubvya.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gfpmoqhvx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gpdxabefg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gjhumxqks.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gxswciqqa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/glzlfnety.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/glpldureg.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gjqhupsxu.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gnsrbndpl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gsdprfnwl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gfytrcbuc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gkelslcco.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/guknpzapv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gwwphxvnj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gsngdjmus.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gyzsotffe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gkiqgbiwu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/geancicvy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gditnmlkd.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/grisbkfre.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gsixjlrrd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/grvixajoy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gkmicbmvg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gcphubqon.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/ggrxzqhlo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gatwauwan.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gxccukknu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gdhxobhro.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/glxomoswk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtnmovvap.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/guyjlzewo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gyksxwgeg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ggbhbufnq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gcebrfiak.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gmwhywhiy.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gupcxwvvt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gmimqetxm.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gudasdkat.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gccshxkko.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gaandcgal.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gxvbjezul.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gmwlomqcb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gaxkdqnep.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/geccjuomm.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/ghmwfhons.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gqxcaiwuq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/ghwymubio.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gqzrqgacm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gsdwnsmlz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gmcquabdm.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gbortzxbm.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gbadcjiyb.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gptnrakvk.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gjmbsnebc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gscemwxlv.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/goushlkwr.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gzmpgauxy.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gwhiafpuv.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtptxdlps.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gvcezeoyc.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/grovelexl.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpqwcscxb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gqsklttev.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkqzkblog.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ggjocryfb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gqovaulxt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwnspfyto.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gavmmfksi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gyxulvvis.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkywwlcgb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gbwpseebg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsgqwfcnw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gkxnkrdob.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/ghdfgggyn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gkrwrrtfq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gxtxabxro.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gzvfucgjk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gcahgdzub.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gkesbykuy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gchsumqll.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gsrcwgzus.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gpevwoifs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghibrpbaq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/grdnpapnw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/ggdkthqzw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gbjrzyoms.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/goqqhjych.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gwqsegfzl.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/golhdpxgd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gvmwhqdpl.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ggaxznnej.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/grozmdizy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gxefltnza.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gvwvwibdq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gmbviutvz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gwsjqocpa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gfdpvbmpc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/geknzqdxj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gjesqxzoh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gxbaagnmv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxakglqfy.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/glgkantmx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grmyfulcg.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gfpiuuexf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gittpmnmr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gbiwieytr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/ghqeggfiz.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gqbrqbygi.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gjmwbxcve.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gcszcymib.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/ghykoqtjr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gjxhnkyap.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gxfhqlvtn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gpgiartrp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/giutxsbho.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gtayeibou.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gsgdaitzz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gpvtyocjb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gsvegfsnq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/golnmnile.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/glidzijij.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/ghjwxozuk.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gepwpfjda.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gelsgeiyn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gpzoshdnb.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gpplzkoqv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gwzmkdguv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gsonmntom.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gyljtjgpo.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gogulgjrg.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/ghlmulejz.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gwodrcahw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gfehfffsj.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gaaeikagk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/grigpqpir.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gebyezfnj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gwqwsylmb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gucitcewj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkcvuculm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gobfphlad.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gvymzvbba.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/ggyolvhgo.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gkrizodqz.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmxxcsbhg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gswudayrt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gvtchgehx.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gqfddkhmz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gprusumgn.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gvvpvodsf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gxmefqokg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gcjbkqjqm.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gawbdqwdo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gjgcqnxwe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/guydpuqzo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gnpseczjo.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gcwxtehqz.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gpnozdsar.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghhocpwat.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gohinaiwj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcyjcncun.sHtML


<!-- 参考信息 -->