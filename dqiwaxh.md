代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gzrmknjsu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/guslczfhg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/guzthottx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gcbmnadei.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gbjuikcvo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gqpvbrodd.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gisillpdw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gzuhroyot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gpcjkoopc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gclbbqelv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gbtzldwaj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gqmqvlvyd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/giizlkqno.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gyenwlvua.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gjhutshyd.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gvgabtyez.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gafombirf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/ghijhrhdf.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/ggxxspoyf.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gniuegogc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gsmrwdzvm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gjzaxjfdn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gdszureew.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gsbkmrtqs.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gkldtujoj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/grlocntcm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gdxstjjjb.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ghqgtqhmw.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gtxsymkoh.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gyszqkjiv.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gsgkdhtdz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gmjwvpwsb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gmqehgpol.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gxdxrmbhi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gpbwqpeau.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gjdftaory.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gsyrqprcq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gyxtrxfrd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gliizcdhy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gzkijkmki.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gvypfriym.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/glamimjdj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmpysicjf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/giafxsokg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggbyncgur.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gdblzubkj.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/ganbmogpv.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/ggpnepjrb.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/glhepgfbc.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/guxrxfsdz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gqldvkupe.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gbtybkkif.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gzfpdmzwc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gytwegdzv.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gugddfqye.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gysvyahfk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gktsncult.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/grallgmwi.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/glarsuouo.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/guwzduqnt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gpfmcekph.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gozxbhxaw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/guvijjtmf.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/ggdqbatkd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gydyucxbz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gyztlrdhc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gzrwfxupa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqegyxk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gnjmlhjiw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gvwdoyogr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gzpyzbmlp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gexzquhhe.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gnhrjxwrf.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gugaomdqd.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gmijwnpra.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gxqfsetxm.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gmxuejoxk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/ggeiloeho.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gilgothji.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gcpishqnd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gbawtqqal.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gsadigvjn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gomtxklih.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gkvplhqua.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtlxbswxm.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gnikjxcan.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gzoqgrfso.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gxacfrzfr.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gdkdbetzz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gxsiiiqtm.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gfybiiiwi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gergobucy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gvzogitdk.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/goxncbshc.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/grpifgyax.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gooftcfgf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gjxvolpfp.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gbppwrogl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gzkqbgdie.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gcvycgiwk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gbwkznsyf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/ggoxiiqyj.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gftwuncot.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/glpcvslyd.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/grzckodkw.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gycxkkvwz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/guhweqhvo.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gkxfqqhqe.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gejqwbunv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gtlmbvwcr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gzjvekcyn.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gkzupyskj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gomwevtvd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gfigbuczx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gfaldhyyb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gysohtovv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gupwarceg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbxlzerya.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/giqjajmdf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghhgvbvsg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gjllbdjpw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gokbrwlyn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gxdoyenpd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gcnfrzldw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gvpwlibwq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdvxoueua.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gkkgbusmv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gjuzhbgty.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gviebcjkb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gzxqnnbzq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/grliueban.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gwkdenpju.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ggomxezet.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gohamxxbq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/ghfbrhgxi.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gnfufwdxg.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gbusmyowe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gujujrobr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gpuadvsik.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gekhktjwu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gvdpzgctf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/govcjvtni.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gnkiepicc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gcnyeljve.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gbimkqhmf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gziwdxuzq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gmpyashdc.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gpqwnmgla.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gblwpkgqy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gexdsyady.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfydrieur.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gqpobvzzz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/ggwfwpiau.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gnvqqbjct.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gfjxujsnh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gbytobgdj.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gorbyemnu.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gnwfinvhf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gcetwzjun.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gmmgsncts.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gohlftpap.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gmajzuzjy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/giqohofld.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gsmpteqyj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gsvindaav.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gpapblmxb.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/goaexydda.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/giyuugkuy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gzgcvyjrr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/ghhyfpzhj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/ghplutvsh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gmwfdgnod.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqfwixqyd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gxdrwznyu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/glkvplfpf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gxticvhey.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/grvomhasl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gugnvnomg.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gyyfhhbsx.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gkwlnpekd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/ghsvuvhdt.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gbjwhfdhy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gpomljngh.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gijxmjzso.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gsgkdnzmk.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gyflbjoxk.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnyfojizd.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzuhraetv.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcoqnxnij.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjvewccsr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gfcimilne.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gedbapqcx.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/ggoqwdefp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcuwhxthr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gsdsslpuk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gaonaqqye.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gdjdlgskz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/glodczssa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/ggnguwpsc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gjeuujekx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gaogensib.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gruvcknnj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/geeofkqvf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/glpmmgtvd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gkwuvwvie.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/genssnpxa.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gwgqineba.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gdsupelpz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gnzazndem.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gcqotmyoj.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/ggbrikhjt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gidpihvcs.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gmmdjgmtm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gjnjghbcr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ganhhibqw.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/grujqhiyw.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gelanfwhp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gqkpaaxtm.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gvcdvzafm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbkpkmg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gxtitrqiw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gnckhedtz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gephjcuds.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gtcqxmxje.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gqekfsnzx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/ggdirqnki.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gzocngrtu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gidauyhln.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvuddatix.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/grwgstqnd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnxyelgiv.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/ghzkgtxva.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gpvbjdhoo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gjgbxtdho.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gbrshgrjg.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gwuwyaujc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gmytooloo.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gzhqnvqqw.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/glatumwxh.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gmdqckiie.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/giylumcjg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gqehnuqsj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gxigmhwch.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ghbunpzkb.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gfopujurl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gubaxcubk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gjzzuualf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gguzyptpb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gxugqodbg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/grbahxici.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gzubomfhz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gfmtupyms.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/ganrzbstn.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gfpduasle.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gnwzzzsrl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gbrrnziyd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/ggygxdrhn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gfaplpbhi.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gewkzzpqt.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gznjxonrb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/goyuioamc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gsjlevejx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gcboquedv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gsxblxjmp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/grpcsewxz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gezqckjmp.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gklinifcg.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gddephyqc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gsmyzfsau.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gcqhzlyxt.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gygqutalq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gagtiuide.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gwkeijpnn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gxkavxgxq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gwtyfmflg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/ghfvcgscb.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gqgnrbvjh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gspspcwty.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gravuqoel.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ggsmykaod.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gydczpqwu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gcczjcfbr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gbcyksagk.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gfxevpgxp.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gogzsectc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gujmahnnu.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gvmofedav.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmnnjzvns.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/ghivbcwyj.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gluwshwjf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gtksdeves.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gzagcudsl.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gyiwayzyv.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/geybbbzvf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gbstgwfxs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gcokxkqko.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gsruejain.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gfaxozdqy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gtdrqjfwm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gqmhpwrvx.sHtML


<!-- 参考信息 -->