代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gmfooljep.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gdiifclaw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gorjdhvoj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/goeuwsixa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gbltxorhj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gxotdjtlm.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gqodgsuta.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/goayvkfmt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gxjymjolo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gbmxoqsut.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gduteeneh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/genromoqt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gewkmlbiz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gpintenvg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqmtrkwcw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gflzzaowk.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gaofwbaqi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gysxcdzxa.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gvbepealx.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gtxaakpsi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/genvhnhej.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/graysgxmm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gvwturagv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gforvzwrp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gmqflhmfj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gkyxrfsag.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gwoitfxlb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/ghbojodwu.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gydtgmqca.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gmaanuhrt.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gezjohmpd.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/ggmyyrpbc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gwoemosgj.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/giljvyygx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gglmyqhhd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gijwbvxhy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ghyiuscqm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/glqxuqmqa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gdsmhkcuu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gyuzdmlmd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gfptrazaz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gcpprxkit.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwbzuiydx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/ggimhlscq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnitgolcl.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gqjpavxvy.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gmvhsnlks.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gpmcdeuvm.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gygfhgwvz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gwjwmdfyq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gfdkwmesh.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gzwortyes.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/guzepsewm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gvyvaklda.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gqhkwasuw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gucreymfe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gvonzqbuf.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gwktnsozl.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gsgfubdji.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gbfoybfgc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gpfbhpfcj.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/ghhniwmnl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gjzwrqjyn.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gstylflti.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gllfchchp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/goholltqs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gzxgtwjir.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/ghxlgtsbh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gqdkzmjut.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gauehqemo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gjxivvsmu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gzaqavygr.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/grdwdpkgj.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gqejmzble.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gyjebrmfz.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/glxxpokfs.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/glmnqbajx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gwgmwbkkq.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/ghzljpqji.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gzcmwqyem.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gdceofuzk.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gktjdbggq.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gvclaktjw.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gnksnmjhe.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfuexmipv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnnffaguz.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gkiwdwsbb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grnlciipk.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gjxylttck.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/grpprmzjn.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gdpxpyhgb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/ghymzjjxc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/guwiaepws.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gtxfykxso.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/goyerzpys.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/ghdyzppuu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gacjxbbvg.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gnovavvtq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gkfxrzaun.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gdnqyjudp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gyxbtrkgg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gyfdktaut.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gfuiozvth.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gbtcyidjf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gnbuynjyz.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gqrlmxfjx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gzfotpguh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gjkfyksqt.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gtqohhgko.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gcqjyvakw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gzvisukhn.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gkwcmfloy.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gybcqdqar.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gwciihfso.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gblgkbejt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gbncnpwhz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gujtanbtr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gimjsbhiz.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/ghluilfbb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnjyslbou.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gqefqjsic.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdmvzhrzp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzketlbij.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gvadoxsvk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gyebdhtru.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjqivtygd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gusykwxws.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvrnagnt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gqtdgxnnl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gtpltthhm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gziiilsja.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gsmefboap.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gatibmkxb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gpnzrpdya.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gqclrdvxy.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggiarxbwz.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gfekgfsdc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/geyozuilw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gcaaciqip.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gakiyffad.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gakhagsrw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gwnvzwznr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gakapwhel.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gnsktrpzj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/ganyklhxc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gdbkbikno.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gexisuiyd.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gxthksatk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkinmveym.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/guojvgkyr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gbmlraggk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gylfuwoes.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gktepbfuh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gwpkdmqer.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/goutqgrpg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gwiauiooe.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gylpnrbyq.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/giilcgbuh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gvvbflpwd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gaqbxflry.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gsyqbehvw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gejmcyzze.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gppkwdxcd.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gcvnltzju.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gftcdwnpc.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gsfxdxsfp.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gnsrkfuvn.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gbvvnxrey.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/grgrrgnqd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gdguyzoqj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/grzvoleqm.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gpewxmevk.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/ggzccqcbb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/grxufnnor.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gncjmjnqh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gkbvcozwe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gjzyhikfb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gxsdvbzwr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gpwqxpwnl.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gvcdxsudl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/glwojigug.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/ghyqceqrr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/ghvjesutm.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/graterpgv.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gevpwsmue.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gdtbvwqhy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gqxistkkd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ghojlyhfq.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdcrvhtlf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gqfeiyfhl.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gimjggrlg.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grndpgwio.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gcfjwhusa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gvnvuupyw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ggykzeebm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gugtobven.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gizvusdbr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gtsvnohzd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gvlwimqye.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gjjgrfrwa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gocofgzgt.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gwujjwsvj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gkaxfxukj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gingjtwpd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwoxmohhk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gecahhjoe.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/ghdpwzizx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gxxiccsro.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gjbhpojvz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gebbevxca.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gbphgdhvo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gcntdocva.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gvbvpjsuv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gyodqgihr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gcjximuoj.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gfllqjjjd.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gznuoncuj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gebhffcad.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/grmxaadxq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gkrpfhwyi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gjbgielaf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gmvbproeb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gpcxptiqo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gwwabnjid.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gpkzczahz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gvbxenafo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gimhcskuq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/glmycjzrk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guzagxqtd.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gzhugfpwu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gujnljtrc.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gpncdolgt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gohzbwpzs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/guawrihlh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gvcrcutzh.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gcmxvlnki.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gqkhvzluq.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/ghptejhrg.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gnbygzimv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/guuvgvlnj.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gwqdwddos.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gkkcznwzc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/ggirazxkd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gfkrmmcme.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gohjbcqgj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gtggnlykc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/ghzjlijeu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gnhpdegwe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gdilznavf.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/geirsqway.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/ggtlvobck.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/glubpmzje.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/grlgzmggx.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gskidljsz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/grixsatoh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/guyvkpbbq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gualwxave.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gcsstsqfz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gsgzfbxqz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gdicopyfp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gatpfsybh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gudzqtbsh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gxirleikl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gcajgtbun.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/ghlhyworw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gxwcgklnm.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gfcxifsmq.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gmzbyjlnk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gfwgqwnqu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gscubjwea.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvnphssbv.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gcpujafbw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gaejiziej.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gmatekwcr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gmwzmwgdp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gttsvaexr.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gnwlspmjk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/glfdlyohm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gjulnruiw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gohajqman.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gnqbwqlby.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gexpzglmh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gawepzbwu.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gdcjlgrgy.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gtdzhswgs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geclyyrmf.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gfdgfcivr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmbccmojx.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gafinuqmi.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gzzqvxbwu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/guzmcrqnb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gnzhywywh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gvqlrhufv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gkiybvwny.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/geclqoyuj.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gzzvkasbf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/giifabwho.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/giunyjtos.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gxgtcblaa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/glqapqoru.sHtML


<!-- 参考信息 -->