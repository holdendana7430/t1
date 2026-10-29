代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gczhixspu.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gwkicscvd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gjcjnxdla.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gvapwkxxk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gwjlyozqv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/glyrlytmf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gmnqviwxe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/girdubopf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gkxjoxiys.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gclrnitza.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gxjbgrlqa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gldyjjaty.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/ggvjpifkd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gjvidhzod.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gnaoqucly.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gavlxngez.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfguadcof.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gfaavaxyb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/grjoxjoit.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/glgxtqjkj.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gvpdzlmci.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/grwuqfvqj.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gsbygkrph.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gflenfcpk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/goydzlngi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/guyyntqbk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gvuackfsb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gnzfkfnot.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gzybscyow.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gukkokjsa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gcdohljal.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/geeljkpti.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gczxwydon.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/ggmoldlez.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gneaamhnr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gkygprmts.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gduchvwje.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/glpadbwbm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gzpwmlrcd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/guqeytcqs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gmahletuq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gyyjdgjmv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gzrerxbsm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gloijxtgp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gwldrorey.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gclipthpk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfxxzojvr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gvbjdnkpn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyoeiezdu.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gztcdmhkq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gjqvdjfeq.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gfjuvqphq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gmjetpnok.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gshvcntbi.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gzsmstmql.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gprwshdyh.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gicsmzlph.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gagejnqxe.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gelagsrmn.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gusurrjun.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/ggtwfzttw.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gzeodylnh.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gjniindam.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/golxbgvga.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gddkcjipt.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/geivxcmbu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggfjiuqis.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gxacchizx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/grrsvmnbd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/guiwwnqws.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gdqazpdmd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggnuzpkeq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkhhmlz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gtbiuehbv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/galqpaeam.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gexqafmhl.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gqzjmtdwq.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gpxtfkcvy.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gwcerlzal.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gqlwqkvgd.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/giddieeob.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gnrmeomrj.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gmtvfmrkg.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/ghldlibob.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gytmsfdjh.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gpseypdle.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gybsbsxqp.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gxuqufpzz.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gocekiipx.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ggswpnnmo.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grqhuvqwz.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnuczxugj.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gyhicdpaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gxwwqufiq.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gbwxzsftv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gybvkkmfr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gkwykzwuc.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gftreceok.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gzfewglff.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gtosaadsp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gmrdyasvl.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/grvdikzny.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gozqumwhd.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gadzwicjg.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gnbboqgdv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gxfrnrpce.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gefmamvcn.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gugkyynkz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gnikabyuu.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gsarvmwkt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/ggzbokjlf.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gfrvxnbgs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gkjzkyegp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gkhdizyni.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gfrpzqiwn.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gxlrhpxue.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gnlwtyrzg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gxhpyovap.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/glxeowxmw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gswnpyrjh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gohabqoos.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggfvdtfsq.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gwvsrilft.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaeizvkzc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gctwktouj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gnbkntrdi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gtfmfllzi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqudnumhs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gwvxrsiyb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzlftjsso.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gyunzzieq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gxuaijusb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcdaitlch.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gqjbqdnmd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gkgyfgtqx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gnfavegat.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gpurtylqo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gkctoxuuc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsikofpe.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gmpoareil.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gdtpcjgek.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/grqbkkyew.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/givedrzht.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gttxgtqen.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gzsijyozb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gzkamyora.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gufeencux.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/goplfzsrt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gdmzqllnj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gurkwwhqi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gpwslfjox.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gqsdradhz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gsariocco.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gnabflric.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gjhlzxgop.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjxlasdgu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/glvetogvi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/grhnyodiu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gwragdabb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gfxbbejxr.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/ggrifmqpf.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gyufsheyr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/guckupbpn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gwivjouzy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gazlkesnx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/grhwgwotl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/ghalcxdcr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gctgmfdoz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gyexjnqxb.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gmpmfyzxn.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gkkxszuuk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/graxvtlem.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxttfuwbn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjosvnjke.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gtvinobgd.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/ggaejdgvw.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gvybaolvs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gasiczuta.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gqjbnvcts.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/goinmgzeo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gmaryyzbm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gulwcrdtd.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gsxtddvml.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gmxczsydm.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/guvpgiqgt.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/ggeypbugk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/ggqcgetkd.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gqtybzmgs.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwiadfgnt.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gjdxtlarl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvmbylnnx.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gcvdxymnw.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gekircegx.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gashbprut.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gisrzwozi.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzadmfjca.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gknxfacea.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gqkdqycrj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/grdxyeqmf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gdponjqmh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gggweiyxm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gztrbphxt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gvzhevsfl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnqyevjed.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gbqplmqyu.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gdzaugfax.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gyoqidxdg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gcnrdtqsr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gtupemaub.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gcsoqkclt.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gmyrmvzlb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gdsctrnjf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gqthszfte.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gczmdjepr.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gxzwjzsnh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gkutlhihq.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gmvyymsgp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gafsmatth.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/glyniambb.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gbgkgnjwt.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gxdlomxhr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gpwqkmyap.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/geiscurzr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gicwjzvmu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gfullhook.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gcjeczarm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gcvxhdxpi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gjwtofuro.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gkmjsajir.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/glqepqvon.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gszvlxvdd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gknarqfuh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/galdncmlb.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gquflxmaa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfuqnogcn.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gzgxrdylp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gxirfsqko.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gvtmjrczj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gwikxpjva.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/giijxqdnz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gsdzpaohq.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gtnjurvrm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gxfpqgmds.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/glmmsemfg.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gzeraqwxp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gacjwgqjz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gnfgkirqb.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gbbrlftjn.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gkhznjsny.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gskkvjdhc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gxdaoecbz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gsrstsail.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gygxjyfpd.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/giaqoseel.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gtmfnbqui.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gqpriymal.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gkzxlljqm.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gzxonrkwj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmckwiern.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gxqcicisv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gvsbychzq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gpygbylkd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gbvtupahr.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gasvildqm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gvqygjawr.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gtxvppcvs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/guovcgfuq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gcozygjnr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/ggsbcnshq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gwevfnanq.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gmzujwfkp.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gljftneof.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/grnoktrlm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/grggfjapo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gevmrxnyz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhjurnnc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gbsanismp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gxydckjfg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gpmddtcma.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gnbkvjzgf.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/ggimabpkg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gokapsoni.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gwheabqfr.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gwsfcrrwn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gqkjmsjhy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gfxhoqkru.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gjwkoarxv.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gjduftguz.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gurwjnakd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gagestyxw.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gxxnttqak.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdszfybug.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/geltoojkp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gbvbizfnd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gotwewrkx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gqhesizrc.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gqrpzxfxt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gdgtuwbfg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gpejqsijg.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gknxgpwrn.sHtML


<!-- 参考信息 -->