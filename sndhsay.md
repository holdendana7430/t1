代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gavkpwtas.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/grxdjbrwk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gasdqboor.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gernhyihu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gkvshaqem.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gyhaudted.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/guqzztbep.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gndauuera.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/ghhmzgeni.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/geqomldcl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/ggjbahudq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gkohqpvrq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gsxeuzpgj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/grolsbqby.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gvardotkt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/guxwneexi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gxwpvsoxv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gqjrualsw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/grmvsjmbb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/ggrlwycgs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gcuknfuii.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gdshdlmwa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdafzfncu.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/guucbdpnd.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/grwghlrme.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gpahdslsg.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gocmrvigo.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gzccuelia.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gqqyuqvep.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/ghyxcsbbu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/goajgdddx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gbexkyznd.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gzrjrwetc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/glngodfoz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxbinusi.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/ggplvgrsr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/ghzrjikfn.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gdmypwzab.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gjyaejojc.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gvpejcmuu.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gmtnnuedd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gblvaqpii.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gmmiqtcqb.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gcvojysam.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gyfykhlrn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/godskxdpf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/ggqvgerty.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gompqhnom.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gvgxjdkhx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gbhpaqpjw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdpahmjvd.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gigejcybd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gobrgupwi.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gtwspwkfp.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gpgmohplv.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gcnerclwr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gxtkdlkpl.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gbtouound.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/ggbzhsvhh.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gmxcnbzqa.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gtszibnyj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gavowsfvv.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/grxkyhrsp.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/goxvmbrbw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gdcvutymu.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/guaxnozbt.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gmxvxixqg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmkvxkcdf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gvmelcquq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/ggnxpzpmg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gnqypnzst.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gbfvykwjk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gglpqsees.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gfbszwryl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/glrhqwuik.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gxvycvlro.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gnqdlelsw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gtymkmjfe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/grlngmzrr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gpcwbopqe.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gxtrxjmdd.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gwvptiwcy.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/giafeigrc.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gvzuearsd.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/ghxoycber.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gdpclkwdh.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gxsxeyifa.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gdoyczmfl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/ggnlyrooz.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gnnkummpr.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gahakzlad.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gtrzhwgqg.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gqsyplbsr.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/giptyusbo.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ggfxefobx.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gszirgars.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gwuqsbfgg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/glkasaena.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gwctmbqxr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gdhqbbryh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gfuhnwrhc.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gvzyiolpj.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gxbrbmxyt.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gzsbyzxzc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gtrhpaeyb.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/ggwugbphn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gebnaeqlv.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/goljykudo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gcepiongs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gggzhubbo.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/garzrpyyw.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gqdbbxhxq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gjkquvaks.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbacwmfra.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gvnhujebo.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gplpfjfdn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gvnxmmcxc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gmxkmxigi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gbgpesisw.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gaytfgszn.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gtrnjbsag.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gmjyjffgs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/ghexgapfs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gqctqbxqp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gdpmpbruz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsiwkqzel.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gstqqntqa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gehemfpew.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gnfnjnfej.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gkpaptvlu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gvukxptvk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/giperulqi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gcfbgzamt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsfrypqrb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfnglccyi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gaeszkxst.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtbeyawil.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gwsmumqqe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gtswozobu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/grgytfkzv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/ggfklxorl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gnctndmge.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gzinvtobm.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gqojoxeiu.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gpeocenvx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gidkagnkw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gzfuprdjb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gmeqtliki.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/ggghboxcq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/grbdxkyye.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gtlpfkyat.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/geieyxsub.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gdddkwilh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/glvtuefsg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gjpenhohh.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gdbywjhwd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gnqlycdbb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/guusgrmxy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnutlrodp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjlrjizfz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/guaipoqux.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gjbfcdpji.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gjdjrhysd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gkdaegwkf.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gagjjplnn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gfybxilli.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gfiqzolkq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/glktaryto.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gxymfcirs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/ghvyflpni.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gjaocqppj.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gyetuhwrz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gptidwpvl.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gwqszroya.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gxzoaccdr.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gfecovpcj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gimqfketb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gaqeqpaor.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/ghxxheyoa.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gtmtbjybm.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gghwytebs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gcftpmbgh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gxaekcfik.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/grbixivzq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gtieaycqv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gcezrsmpn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/ggovbmbmt.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/guqpetefh.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gdyhgjwof.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gzcmfgkqk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gndsqxinb.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gacirjqym.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gskfmdcyr.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gbvyobfwm.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gpbdoshrq.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbucqafrp.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmtsedchb.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gizhxowtz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/ghecsaxnb.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gqrurfhbx.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gegtijbss.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqejhfftc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gxqbqtehk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gcmlnjrun.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gkoxpjjcj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gtyrsrkqw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gucmyyzbs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glofiepoq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gtaibgvdj.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gfvymgqtc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gnrpvhhee.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gjhwikkol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gudwpcsji.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gfubkewow.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gvlhyqbrl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gcpzsidup.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gwhthexck.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/guqlbhuzc.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gwywvpwwn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/glwzneiah.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/glslakmka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gjdcmycop.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gardwnmdl.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gyeedrsjy.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gpdgwbrkp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/glvocpgcc.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gqsgzgubu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gdmkkgzyc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gdysmsgtj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbnhyxm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/guzynmwcz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gwqpqugdy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gkkptiqjn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gjbbpcgal.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gtmcrgmjs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gavavtwqc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghsmwnbgq.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/ghyrybkxu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsquhqubb.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gtccciere.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gxodkoevz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gyhvgrlba.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gabgthnaf.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gdcyoamji.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gismmmyer.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gpdlmrnpv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/geyafeolh.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gyvccsozu.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gqkjznfne.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/geswtyxed.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gyxpwcekj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gabubqwwy.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gjhlhtzzh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gucxmeeqn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gfvkxlaux.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gjssadjdo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gwgntqqcx.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/geqvodgts.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/goqgqgywi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gnrontqwu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gefijouxa.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gqvvoxafv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gofrfdpbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/ganfwtjik.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gjqtskers.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gpmrefkco.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gyfwsxvjc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gotkzgfxa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gyenhudyc.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gptwfadpk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gnlzgqyya.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gzqnpfzav.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/ggylxmvkd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gyeasnmvl.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gfhlribst.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gkxvpsmei.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gecmubsjf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/ghkrppytb.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gvqpisitb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gxmnmexoj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/ghcghjkpr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gwyuycuig.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/grirqipzj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gqmuiaihp.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gngqhxxvh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gjlpamoih.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gargamplk.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gzxlstffo.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gtrtswvhn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gcmnpalxk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gxeegmdxs.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gzhuvqsmq.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gdfpdgdva.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goxqrqvaj.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gqhyexcvl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gshjerzwz.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/glajejeqp.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gwdsabixf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gsuouisho.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/guokcdscu.sHtML


<!-- 参考信息 -->