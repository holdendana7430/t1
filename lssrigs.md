代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gvjenpnpb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/govcarden.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/ggrfgqfpi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gtyiygbud.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gmijqjkkg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gfhnbexcg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gpscjtvca.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gsccdkudd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/galtknbjl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/guffoomyw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdmbuzflt.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/glgdchrky.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/grvmjeldh.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/golerdnpc.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gpjgupwpw.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gypuyvmfl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/glnfviefl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gutlsriex.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gszetqiqs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/geglvnlxr.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gvsmdcxij.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gtyzpjimu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gbayihkyy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gcxdvtjfp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gofcdfxyy.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gxyfxqtwp.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gugvuovzd.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gaquzbvnv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gydlcgflz.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gqevhclxp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/grdlerukf.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gkzwhlknj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/giwvlbefp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gqgnzeyjm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gqtnowlso.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gllghbtfk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gbuwnrnaw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gtewiqgsr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaalblgqg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gvcghnxmw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjiqdtfhx.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gigkwhjvj.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gdeudxklt.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gbzcsxcgp.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/grijwbvsv.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gitplyjwd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gqtkptucf.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gphhpxmxm.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gduukynvt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gaxlqxfsm.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gmlwvkhok.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gmvynfpfq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gokcmcvat.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gsinomwwm.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gkbehuhye.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gyegtkbes.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gfwjpzxue.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/ginoujrpp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gappjbofd.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/geaxykqdz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gsxdbtyvv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gtoubtjsh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gwsnpcpgd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gllreqker.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gfkqlvkge.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gaqmowhnn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gwuwldhnl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gyjybpkzk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gymhcmndh.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gdfxxslmf.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gncvbpblk.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gwpyjlmjo.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gdayahtwn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gxwqrjfkt.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gzevucbap.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gfksmhfnz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/glugilvpy.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gndyfasdq.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gluqkeffs.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gwzdxmsyk.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gsvyzkzgp.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvqmxokjv.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gheuorsis.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gyvefktsq.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gcirrhdds.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gqqocjrkr.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gkyalnmca.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gckhgqhrh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gbpdlfymc.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gybfsjwlx.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gkwerqrig.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/ghwdifsoo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gjrphbbls.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gepqwkgbb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gxpcqchdd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gezhahdru.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/groprpoyp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gjxroluyy.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gaxrnzlcf.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/ginnjiutn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/ggrqlgeuk.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gqurqcaxl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gcaajmqsd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gjkrtplko.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gqoqbaamb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gagcxozbo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gfvkjurjp.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gkokrimwq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/ghxgbpyoq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gsqdqnbbt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gyeilahtb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/godudzpue.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gcrpdnrlz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfjlxtrwr.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gvbbijqul.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdtzxcsnj.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gxkepfgci.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmvkzryde.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gjnbjocso.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghaapipqh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gdlpvkaqx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbysjurlf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcdowkmul.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gevcrhsbl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwlywcdfm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/ggnfkxnai.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/grwldfnud.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gawztjmna.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gauipnpgf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gfkugyxab.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/goaoggphi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gytouwias.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gyigokxrk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gmhqpbbxx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gtvtsfwmm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gqkoyodkv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gexusrtha.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gcaoasmep.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gdadunszs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/geltecroa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gpksztkld.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gtzhozlje.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gdzpkctja.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gxjsxjrml.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/goxhkusdz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gemqdplwa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gbtgwxwfc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ggsygwzci.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/geejyrnsv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gakrkwqtt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gladcxkkv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghmfnjjla.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gbwfkrrpf.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gjxqahrhk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/glfyfqnkj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gswqsgctl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gejsrgukg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gujsrkemt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gwpggxkvb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gnawqnnbz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/grzagzgvj.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ghhkcsaaa.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gzhlslyar.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gyoyzzuml.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ghixkdtci.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gbvfwddrc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gamjlcunu.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/glzwbvmfm.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gohkvnexd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gohaxfjfq.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gfrtluxeq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gubewtwuy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/giggbasgv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gyayfcoib.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gdfzeiujo.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gdglxjqir.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/grsuaxyqa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gbaocdcch.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gmbflobfn.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gwylxesmb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gucopsqhx.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gztnlorbg.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grrlqkogt.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyljrqixc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmgizqhle.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glbxzbszd.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gjuifbwzs.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxyfmnhpg.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gmftxieof.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gtghapmlc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gmxfnrvuu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gibwvjldg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gvogkvxwx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gbeaygkjd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gszwevxxh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gzqiundcx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gzzqvwojw.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gxbfqvwkq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gcmypplst.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gkczevxar.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gepfakqet.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gljhlkbqn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gfafvdygd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gfocpqejs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gxivuedbn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gcahmrwwi.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjscqgvxo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gsbrfnzby.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gcugmwwkq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gllezpqwz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gnrmcdwbc.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/growvmutu.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gmqmqopzx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gzrihgzks.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gpfrgescm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gmivjmyab.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gopwleisg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gunplnxay.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/grruzjrzo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/ghhtgtnjj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gnjqtbouc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/guuissyvh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gjdasuvdd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gyazilvch.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqsdtdair.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gmigrwagm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmxgwziqp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gjhgxztpl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/grqerkrue.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gbebewrpu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gmgynbxni.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gcmmwnhhe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gfecrqypu.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gejvqcqif.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gmbjtfbmj.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gebjwlolg.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/ghelfordn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gdewulfrf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gwklhppie.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gitqrzbdh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gdaxdpouk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gytbfiuuz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gcqnrnhzq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gqarkxixx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gjjizdukj.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gwedhgcxi.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gpfomeoib.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gmhmrklot.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gsfrldzpu.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gpdvsqtht.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/grqvlegbf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/glrdustvp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gqqvxfilr.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gkknusoqv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gcqzwuwza.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gsjzbxcuh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gtvcrqurb.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gtnlsqngz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gejunrrzh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gddwzcoiy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gwxtaxwbn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gmaxyqtsd.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/ggurvwkjd.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gsuynokmx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gabdswwdc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gyjcisbud.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gzhuxestr.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gfrmphsez.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gtumkgtuz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gljejdkzi.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/goqcxdfle.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gkfnamkhv.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gvakvoxpp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/goktcqouj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggodtnhxe.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gqijlpabe.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gpvjuctan.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gcrirnzof.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gaiaqkrcr.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gmwcauvyj.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gusorswcj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gftgrebza.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gbyzcuqbx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjsddwahk.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/ggcrkwsrn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gkblrftwd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gnllfpmsz.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gpeicjjsn.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gjefjjmbl.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gipipucrf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/ghwlehvbn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gyanzuyyr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/ghpytdwvx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gikkwsixi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gbtejlego.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gvujxcpsj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gkdvwecou.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gwjknbeaa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gzdfymrdz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gyugchgmo.sHtML


<!-- 参考信息 -->