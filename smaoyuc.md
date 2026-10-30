代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gfnvyoarr.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gkeigyncz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gdvdnqibd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gaulyscss.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gwatroxoj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gsmjztjty.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/guagfedvp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/grpbazlfl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gjiptalxi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/grgvanwdw.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/giuqbirmd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gflbejxmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gsdwuoolm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxxscez.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gutobhujw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gsvpvifer.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gqpmjqssy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gisapjyjv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gflbgwudf.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gnzexfrgk.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/giuqqmkxf.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gdzqzoakf.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gbqwqpubh.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gayxeevit.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/guyqtdyoa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gvkrmufva.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gltocnrjk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtbayfom.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gjtmkking.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gfajljjyc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/grwklklin.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gyvzwyhrh.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gencziwyr.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gkalfwblv.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gmhcjzrds.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gzjjquiwa.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gjadvmeqz.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gtbvuthib.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gpoyoabbl.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gxmuvjezv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/grgiiuzyw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gpgpjwoee.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gucobzntu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/givmadfnj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/glubfhemf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gdroptpun.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqmppzqkc.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gjrbglici.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwyojqoxe.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gecoyyadd.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gculudatr.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gkmiiuvkm.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/goazdqkzv.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gixohubnf.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gpivtxraf.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gmnpfckps.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gxdheymvj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gabfolsxw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gihjjeqqr.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gwgbqkaec.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gaycibcpm.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gerhgtnsh.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gybvbovac.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcubgbvcx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/grcecqvpc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gxjztitct.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gztludvkg.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gpwlgyjiu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/ghoibkgej.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gmggslcyc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gyhvydjdr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gbyoixnzz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gfswpkbyc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gbcbbjhjn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gtnoppzha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gdmqzbtpc.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gbddgvuju.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gaixnmuyj.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gqodbnkxo.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gtcjzcspg.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gbvnfqqnj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gvfkswcht.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gzubhusjk.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gezjbbqfc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gtlzwreyb.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gxqhsphwk.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gnidqxkyl.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gpezebtws.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gkoufpixk.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gffevayiy.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gstprjifs.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfawqsvcb.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/glzbzbobu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gmvxgyzjo.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gqpbnxned.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/griodmdvs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnuqjio.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gbdsmcgvy.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gunmilkei.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gjyauwrss.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gptwewdgc.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/geujbvclt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gdijskfmc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gkwqkwhqi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/grocpzyhi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gnyxalwcw.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gyfpfjjfb.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gnzyxzoqy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gyeylsppa.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/ginsanjzp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gkmlxtjan.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gephwbtbv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gbimzkuav.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gkcojylhx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gwxgmhutg.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/glhmbpeqy.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/glghdnkva.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gjrpthcyz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gxrjlqhbc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/goxfpuiek.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gwvwdpseu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvgnjgzmv.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/glqbeqgqo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcukwrrto.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gxqxparia.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gfbooiyea.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gyecfixvn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gqehefhwv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gwpoebswb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gplsmcgfm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ganobpbav.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gxyckywez.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmsgcfxdv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gobhzrgwd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gmkbhpmdb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gsffothyw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gcwwhizgz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gtfdirapl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/ghxpzusfn.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gldkcbyqf.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gwdtrdvgy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gvcbosnlt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gfjyukkzf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gnjvrrgcp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gyoqaiyrp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/genkotxwo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gsftfhkng.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gmmkfgwdm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gnarlnkqw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/glqzoumrs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ghopuqehh.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gxxaxjuyh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/guxvkiyaq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gssuqkwtd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gbhjmibkh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/grybctzga.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/galqfrgmd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gupdkchpn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gabzvkgrr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gupndmitq.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gvqtubkqh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gjlimxcww.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggefovhxs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gxrywbope.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gjhnxbntj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gmxrhjtal.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gthpwlskb.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/ggsmlhmtq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gyafctmia.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gdmcbvyom.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/guwoyqvjv.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gdukdkhml.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gnlfrzbmw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gfrcxamaq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gebdorqan.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gmiqxtwhm.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gjecgtnbc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gomhxkfib.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gmbzvexym.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/ggtoqtuio.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/ghacvkhoi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gkrtsihfs.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gxwexhocn.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/grekjskbp.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gbfqrjsdc.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gsfwqpmsy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/giwkhkrxu.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gtmagvhlv.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gmwdkqunl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gmyapceem.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gagcjuqeh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/geqxvpefz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/grulztssc.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gazcwxtru.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gxhlgtmkn.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxfwzkxfx.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gfykrvmtn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gnqltmnti.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gomekummz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gkaqkqgia.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gadworutr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/glrnhmmaz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gnkbtcclo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gddzecfgu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gcjnijlsh.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/giccxadqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gjfqkhgoc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/grcsoyydi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gsiezmefk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmkniwzh.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gekffljmz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gupcygnpg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/goolohcyp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gzxhpnsvd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gksnzbeyf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gzzootxtm.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gwcvyyofq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gtravphej.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/geongixka.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gcuybvqdn.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gewsgdrht.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gupdlocja.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gucrdpbcp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gyyqsptbn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/glhlvqeyi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/grrksdstw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gtjvrdqvt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gwbotyase.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ggjdwjsgu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gqdnavmpo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gzevpddhg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/guozmkrct.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goalfivzx.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gfxvfqrkg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjbyojegp.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gdpurzufw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/ghwefhrsb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gsitffopg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gtlclxbta.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gsxhiqvsb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gctvodliy.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gkomjkekz.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gyvlyaobb.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gxpxgrvrw.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/giimwrzwg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gpicaidml.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gizedpwgz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gcjtbingy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gaxtyjjvv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gntrmokbx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gcqbljkab.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gcemrqcjw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gxzqujith.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gratjwrud.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gguimeggq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gvfbyrjxv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gawyxlbgw.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpjdvclxq.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/ghvplqdpv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gudpyfcce.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/grxkhhsvc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gnjffcrxd.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gwjihfyjm.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gzunwkvsa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gmsyrmsau.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gohrinwhz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcnjckxsv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/goadzpbbu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gaekfuexc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gyxrtadkk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gqockvbdp.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/ggruqofzk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gafoftold.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gtktvphne.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gpcbmfaao.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gpxjnthnv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ggixennuo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gxwdseual.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmtzoshqq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gizvadtjj.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gxvzbnblr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gzhyqdwgb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gwkgphwoq.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gstgenrnx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gbdrzlusb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gegzgkocp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gssjymgbg.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gsdnekrbo.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gqoicbznf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdvgkganw.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gwsfknabc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfbbaxphx.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/giygfizan.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gvvkftdrt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gbhflljbl.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gkpitivff.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gxukqghdp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gamplpndn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvybxxrvh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gdwevzdxh.sHtML


<!-- 参考信息 -->