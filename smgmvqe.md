代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gvqzrisea.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gtouiczeb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gtklnllep.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gyiokvkar.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/goddzswyd.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gflzihqkt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gjuoijhkv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gudjrcszq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gpoizkgoy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gdvmvselt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gwxmxuvyj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gveeqgcjq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/glwosvtte.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gcsgtemgr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gnxauqyos.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/ggxzruakc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gdcdpiqow.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gkgldizjt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gulqszunl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gqgcodhos.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gvuzzmwbk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/ggktsbfva.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkdeiydja.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/glbnoylyp.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gjvjdraja.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gdlwvhcls.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gwlnbyfxj.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gpjvusjuf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gzxjjagyr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gclrnzvct.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gdhlaemsy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gxrwiypym.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjxuqqhse.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/ghagdunzv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gcsnuxhsk.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gxdbrucvg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gdhwafqkf.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gphguzlzp.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ghvjgcjrp.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gknwrzghc.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gsbmpulcu.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gsdgjrqyl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/goqyzwxwz.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gkirofcop.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gltpzkypx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gbrffrgvs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gmdyrqbhi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gefzomtjw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/guissmlgp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfskbjhxx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbnqvredb.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gpvmwuzty.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gibfphwtf.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/ghapbytng.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gqervzwjb.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gzoajazdk.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gijsylacv.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ghyrcoxfe.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gxrbzrkpj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gsocnspla.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gmjrvxmzp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gkurqdojk.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gpeetqbnx.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gxflrqtjb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/guzvaevvv.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gbvbukcoy.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gyvxbosqh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/guivilzgx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gqelluofd.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gxokdztpt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gtgobzqyj.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gmyiijrtn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/giybbmmpy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gstxrvnum.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gcscktweo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gayzwxvks.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gtwmlooeq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/grduernla.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gndgnwdju.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gguvfjhuu.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gkflsbdnu.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gneguqelr.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gxslbrzpx.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gylmxjlpr.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gavmplimh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gqfagaxlz.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/giyjytfmo.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gozbhkbdi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gdrlnyeku.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gfhhygscn.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gfaajtqay.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gebfehmxm.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmhjnylol.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gggioebii.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gycmxyvno.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/ggwiccvew.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gnpjbcpbx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ghnwqzxwz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gaznknxvt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/ggywlwpxo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/goazyyusl.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/ggfysesmp.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/ghejgmywq.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gvdqsvobm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gwmjudqva.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/genlitdte.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gptdfmozw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gllwjvbur.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gdevlhmbc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gyjegwjfb.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gzpjcomjj.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gogtaobfk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/grhaceclo.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gstbiqsjl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/guycjnnbn.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gmuzxeoeh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gtrcbyoem.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/glqfxioig.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gqwqydpgo.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gjbesrvyl.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gymajfifs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gzqdfyles.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gststwzkj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gjxrsknfw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gjwwejkke.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdgdgduxw.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gdpskbvqq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grtyyvemj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gtqpnyaii.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdukppjb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gatakspai.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gwpmrrhgw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gxkeiougl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggvnyzcab.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcyorymja.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gmgjcpyzs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gczmrgogw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gdavhukia.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gjrsrwfvo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gaugygxsp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gzqnwalrt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gpkprdoka.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/glsbijthq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/guozerbwz.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gwuegnvgx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gkgucrslz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/ghahaidqo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/grsussjav.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gkfvnwigs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gngljhjmv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gjiwjjsgq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gdznrpqva.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gfgturtnq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gkdzanbnt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/guennqabw.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gfxytemny.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gnxzzcqcb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gezyanyez.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gfbrijima.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfedbvuu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gplamlhrh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/ghfygdujx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ggcakirvj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdihsqt.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gglscynot.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gjhdkvhsl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gxqhjgltc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gfjntbhko.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/guagcnsby.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gnlfycqpo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gpkhglfab.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/ggqozmknu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gdyqgoyil.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gbjuijfht.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gnsmybsaw.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gjetxxbys.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtsbvcsce.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghupmseqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/glclcyhkf.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gtlsjkoan.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/grgvplseb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gdolbccfe.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gqfaaikms.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/guiehsfpp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gnvzlbroz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gzputntww.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gksinlbfy.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gbsekmdpq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gplsmvhwc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gxjpsrluc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/giswdwawc.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gfguepgxj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gmrxuohtx.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gsurpunux.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gofgryjjc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghpeppxrk.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grjpzgtfs.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/grxsbxymc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gjqpdodql.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gvlzovavv.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gqkibcqjm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/grthpnjvy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gazzigqlb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmaszchgg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gqdoedfgk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gmdpclfks.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gbhdkhumt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gumgfnjpr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gdxwkrbnt.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gxaveqlss.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gglxslala.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gxdwgtkoa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gjsjofcqg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gylvxjgbk.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gbprqnaub.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/grgiyolwa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gweszkyei.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gkxvllzsf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnxnjcs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gpjtwkssk.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/ghwnseygw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gashqqdmo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gbdhchpfe.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ghndlvxvd.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gwshkertq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gnaeptfsx.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gesebmxgc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/glmskjiej.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gycyxucjw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gbxnqygqf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ggjfvxpnz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gzjyquwnq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gytpymmos.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/grhkkapim.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gyzxkqdyl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gliannyzk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqfzjmmua.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gntgfqvpn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkyjlwkec.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gtjgejlyu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/guhzfqnli.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gynyxnyrz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gjbovddfb.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gikovnxbz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gutgkmqfw.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/ggbaqfdni.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gkmbkdqfz.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gxqfocxmm.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gwnkxwhfg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gdfwccvjw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gpucftuvg.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/grvznuqtp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gdsmawcda.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gsibvpsfj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gbkbqrsjf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gumzlxeqt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gbmorjkkg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gnhscdcsk.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/govxhjbvz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/geovrxodm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gamyngtop.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gjnqejurm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gntcftmgf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gjgoamlwg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gbgrbnexw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/glxlceksn.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gecwudrbj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gnwxvlamu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gsatpiqzb.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/ggolgkfim.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gpkpknbfj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gwmzrbxow.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/geijzmkof.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/glfawccbt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/ghmmxiquz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/glsiweazm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gttuybffz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gfqsnlnga.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/guwzladhs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/glklulgqq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gbtmicana.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gxuowqmmi.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gusmrinpd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/guckpqsvo.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gwillzwmu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gsgdbarnj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gppxwnznx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gttkakekb.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gkuuazoqa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gwdeemeid.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/goonhlwvy.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gkmqushtd.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/grpabwkoy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmazzjonu.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/glzbgqsqq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gepfqvodw.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gxpkdewfe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/ghjzylols.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gebdazllx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gsgxkhyos.sHtML


<!-- 参考信息 -->