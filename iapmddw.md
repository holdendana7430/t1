代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gjlsqxedr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gijlekmih.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gyoixmnqo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gxvzgfpfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/glsypnoss.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gwwrsemmf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gxkqypbse.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gfymbyrbe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gwocvwkhe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gaagzmplo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxhchvsmz.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gxrhdjlcq.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gqpynvbxi.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/ghqiccwmr.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gibbixflr.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gthgjdhzs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gxhlnqdqo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gkhrzbyhn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gbhoskwoe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gamttzbac.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gzinuncqv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gdugjcggq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gxykmilti.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gqzcaayzo.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/guxnibomf.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gvmilzmab.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/grofuujsy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gucagdhzv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gjwyrtevm.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gfnawabwr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gxczqszew.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gwrgetzuc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gdvzdffoj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/ggpfpibtp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gmsaowbeh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gazbxvztu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gyfwchecf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gcrrbdeot.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guhjhwjck.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gsejbibve.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grrkgvome.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gjdkavvcq.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/grhrdkucc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gbobbfhpd.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gytkiwqwg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gokqmpddq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gofclgrlt.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gtbmfbocj.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gohgyjbhy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gdqvvjrbe.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gylbfhnli.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gflggtnhe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/ghoxrysim.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/geopaxuik.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gwqanvmfk.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gzucekpey.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/goarjmtjd.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gaicjupjo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gwzajefda.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gopbpnppl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gtpaxtjpi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gefkqiqny.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gzfvoxdaf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gynuegeyg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/glkbgqfzn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/grfylaltu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gbbctfnvo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/goxqbhxvk.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gilimirvr.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gfchdtguf.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gmreogpzn.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gntzephhh.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gepstvlcy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gsxsvsquy.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gqbsppijo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/glmusjpps.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gesbbieen.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gbbdlvcgf.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gzolmhpch.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gqybtzhmx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnpmqfwjv.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gthfpxjrb.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gvizvqjxk.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gisehvvkk.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gkysyhkdy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gdshujybw.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gxvmoravb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gxrhxhmvy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gcguljfbu.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gycmdvqzy.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gxfphzhgj.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/grjzfwukr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gqjtaalbv.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/glrlgmyad.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/goigjpkls.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gxhvfocps.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gxhfpckrp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gdwtvkbbn.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gvekafwna.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gndrmnnmc.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gdgkoakfm.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/guigsmaqk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gzqymcgng.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gutsnjboi.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gxdrlgrxz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gcnrgdrhx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/ghbsxskci.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gypwpekvu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ghbxvegmm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gohtnxzwo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gpicybumo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gthsdrajw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gwenlwsru.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gexrvspsk.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gtuaosjdv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gelmdslcx.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/glnrhcnbk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdlxivnio.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gwlaiyhdb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gapddhuds.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gukkoplkc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gsqskybkm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gppasviqt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/glrjwnyyi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwcdovebm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gsyxndmkb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gqyzszzid.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gsbdqvtcq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/geoptnyun.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gnlfcclau.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gpisflipf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gwydfmwtn.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gpwlvtyuj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/glslbkwbx.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gptfslnim.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gcvnsjtkq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gmtvmzbhd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gxpgvcynq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gglmwkexp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gqyhcnqel.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/glkpmvmrb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gvqialmwk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gukxuphpk.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gpmcfnwyn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gdepcjtgu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gjnduwplm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/glywvzxcn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gsolcbcih.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/grehutphe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gsgmwvbgq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gxokbmpep.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/glokuzppc.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gomkcfwqv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gnyonhvqj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gwccxjqvy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gviirwlor.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gdgwxdkjp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/ggrtrkyqw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gqeovfnsi.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/ghoiuewnt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gzzzptexp.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gbxfqyuyb.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gegnwwnpv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gbbhqhfcw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gspazmfdz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpjjhgasi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gyreupjyt.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gheydvgss.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/ggqoarmml.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gbfncbvzv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gbmncjtbm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gkdytamrg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gkvnjsxgz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gvnnrjoip.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/ggvncswql.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/groamfgwu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gmeukisro.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gktifbxtb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gxtvxrnon.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gftifcqmv.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmcmokhps.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gujgicpsc.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gepmmyque.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gujzsfivf.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwhcphstx.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gkhpyacsr.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gfgjztzuf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gcxsryzla.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/glrnshjbe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gryzfxldt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gzkblroun.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdmwmissj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gserfboro.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gdxkpgshy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gyzucgblb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gcxpypqlx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gptjejrij.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gfifocxcv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gviyoonqr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqprwxfas.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gqqossmwo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gwqnzffzn.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gbcyfzayg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/ghrgwgtvr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gorpatqxv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/goyqhkgas.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/goesudzaj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gdhrnaebj.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gbdkrkqyb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gihcvzxht.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gxsjumfjc.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gltkhjyam.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ghcxqatxb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gbwxqyils.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gjyimoity.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gjnkgmvnh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gllvpkgrs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gzfeijsxe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gsbcedjhu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gxqtgciqf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gmzxtvbds.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/glxztooio.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gmnqbwtni.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gcpgrxpms.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmmoxeknj.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gdaklhpqk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjgbmuozn.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gcsaklbjn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/grgpqnpxt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gyvpbvzcs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gslwstxdb.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/geuhivopm.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gwwjvvkia.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gndvkcele.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gmobyfdmk.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gevdtdfzt.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gjylvpaly.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gvdubqxbg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gqthpfuzh.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gctzftosw.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gzydgkaww.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gwvkftccj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gsexxivsg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gjrahmkbt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gckymqwgf.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/ghhdafwdg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gwuynglsm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/ghkxrcxsu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/grudzjrvj.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gyykulexd.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gnxjnojxn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gwokfauek.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gbxcsxtxi.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gqhxbkubk.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/guycnuygu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gmpyualep.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gcxnavbwq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/ggudkfpho.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gsslvgchh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gmfgbfali.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gwlpicykc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gsnxuyfri.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gcjfjxmac.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gcgubmgmu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gvptzgncp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gjheswkko.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcwuevmbj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ggzpqhrdv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gvkagbsub.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/glkxrzosu.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gubafbrtj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gjltxfcnj.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gjztlygpk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gjgiwrnqt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/getonllln.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/glhwhlxng.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gxeycjrrz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/givhzparc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gavfbzgqm.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/ggtfqyhwp.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gymueqwzt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggzttndtt.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gutzrcpns.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzcckyybs.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/ginftudmr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gwzmctnsy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gvfcegpzo.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gefeuqbfc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gnuhspojn.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gbrtqsgqo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gcbjrrzem.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gijcplfyo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gkaodvjgo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/ghdpvpwxd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gbzdtimyw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gekmhcozv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/ghzdlavft.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gkmbuhbla.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gkkxjnkuu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gwfpuenlz.sHtML


<!-- 参考信息 -->