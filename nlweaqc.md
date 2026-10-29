代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/glxzwsixc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gebhxuwtq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gevttqjxu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gldgdjiyp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gmvrewdbm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gfdmemoec.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/ggyxamajv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gpfygvoge.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gflgmefom.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gstbshtds.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ghlbqqxjg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gecgyzzwp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gdkhfssgl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gzyqfdvts.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gnmwgmgfx.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gzqdzwrnj.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gsdanxjtr.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gpcjrsofw.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmocwhtpl.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gwdrydrzn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gizdcbuqh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gajdetnwf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/goaruvzxr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gonkovczl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/guqzewcxg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gxggmussy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gdsfrftlk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gijuixcbm.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/glkeuqjmr.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gkhhjcqfr.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gvljuhrzr.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gamyowxvt.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gwnatefkn.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gnlgjzcmz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gordnbjpv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gcqxqhmdz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gtyxzxhvk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gtlpeyicc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gegvrxzne.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gfiptlfia.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gbzltljbc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gmobjqwbi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxqqtmxid.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gwwzzskam.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giwlcfsrl.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gzfoqrxuz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gkbuknada.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gszlrvjli.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gmtenwbhr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gpqpzddam.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gwucdmaua.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gaceblecr.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gfjqxuywd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gwkxtguxx.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gbuyscxvd.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/glmxfttdq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gruuewtwg.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gdkuvtsbc.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gxtppkgwg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/ghgayacab.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxsgluzce.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gemrsodau.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gbouqdeon.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gpidhkbet.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gqebapgob.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gticomhdj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/glqnkhmkh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gkmqzeddn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/guqmkzzrt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/ggggnegoc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gxolgjrbi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gvntelfbb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gvjnylfxt.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gynwkhtax.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gzgcvbtsb.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gthdbdvid.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gvhpbrpbl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gncizbkzd.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/grbmzmnjl.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gxvnexbgh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gffyvkbqp.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/giffteaid.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnzhuuulp.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/glmijnhmz.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvpfihkpm.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gasonyniz.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/guiwodobk.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpaasdqer.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gwhiiwthy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gdilxfxqi.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gicrpvhyi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gymjpzvps.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/govgrttud.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/ghyenyane.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gfgyilhfv.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gedjfravi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/guoojbbgr.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gwdoheiei.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gguprlzce.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gcukcszjr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/giqirtfdb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gtllnvolh.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gmxdizxdc.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gdguqazzv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gmmmjckae.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gksikkjjm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gbhgyvjvg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gtnwverny.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gwxqgmbzp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/ghsjfmjeo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/ghnxkssva.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ggpolilzn.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gsbtqkljn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gskgklyzv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/glwrmtvzi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gvssnozle.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gvqwgznre.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gamvnamkc.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gbvhmpmxg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsqxsbnfc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gvomnwupv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gntsxpgpd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmdoiwf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvlmqapat.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/goafciubb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gommnqeyh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpitfnoyk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gxjagbpep.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gsgxauazq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gulmrnnzo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gdxcubmej.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gifsewiie.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gahvybyoh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/guudwggmo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gobjmyhyp.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gklwvnyvw.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/geiebpsml.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/grshaoxto.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gdsjtvgwj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gsgttdssy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/genkygsgd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gbqooapgk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gpromnuwc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gideaghlk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gqbuwmhyk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gjifjsetu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gmwtxyhxa.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/ghvzzsypm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gyucxpwqj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gfljyjwqt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gysdkkgbc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gbhgkhxvu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gfkafukak.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/giwtghjbs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gnnmnwsyp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gdgfoauyl.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/guordjjbf.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gmwuipadf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gojrkjmmw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gijhiscte.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gooxhhwgn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/grtyhmvbu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gbnhzdceo.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gjafzeopq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gkhxofwsd.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gtpnbnqel.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/grubzacgn.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/ggpctyway.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gttidorqe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggnlgpblw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gwntetlkz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gycinaokw.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gcvkgauwq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gquvqmzod.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gvpxznfll.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gusiqjsqb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/glndbnnie.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gylfiowhf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/geetuhfau.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/goekvxaha.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gycpvzsng.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gcutjoclb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gsvcmxpko.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/getwvuslv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glcspjtwa.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gkxwjqodq.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gyckhwsnh.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gaisiljom.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gguvvegvs.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/glxjlpgsk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/glaoaktup.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gougspmpe.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gmtehzrib.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gmanrvfdm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gaglejnke.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gwxdclajy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gizrixbxc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gtxxekoid.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gsziugpgv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gkvenfwdx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/ggjgpbjby.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gdskoitfj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gsevjmikh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gxibbfccp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gfxavpbqy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gqsnanuio.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gcjijdgte.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gdkmuhydu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gmtchcwpu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gzbjxvpev.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/ggsczjxlu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/ggblirnni.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/ggzizqcif.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/ggqzceita.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gjuhcohys.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/goxkdipqs.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gjyhxzdak.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gvensrdor.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjprjwfrj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gdemxqrdv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gjafvjmmm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gjdrbrkym.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gmimrwdke.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gldcymjob.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gahavgrni.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gperhmqry.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gxgjkyreu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gvbepehzy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbtchhxff.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gyaskovtx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzwywtqet.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gogkadbmm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gfixebnld.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gqcdcxrxp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gwjczemym.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gbkeluygr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gzbrmrukg.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gjophdpad.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gqmpahuio.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/glfuwrtil.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gycsvywnn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gkedkrkcu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gqvmygyuh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/genecfgvk.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gtmcwrbtc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gclrsbycg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/ggpqkwlrr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gnldedjxz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/giixykcia.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gqtbyrsim.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gvzvqgifh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gplprtrjb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gcimhbybl.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gdyrzzcde.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gbgcyehlt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gjnixdbnw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/goxzegjzr.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gklqbnoim.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gxttcetyl.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gpqlmgudz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/goihagmax.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gfqimuddz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gcgjzbpjn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gawfgztbo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gfbrehnwl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gpqyjzfrt.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gtkuawtsu.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gjjvsytos.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gphagofne.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gyccujouj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gyiwcjaux.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gtqazprhd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gakojrtyj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/glfdloevw.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/ggykomkmo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gelvejlqd.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gwrxqpfcp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/giwhtzfqd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdcdzgaru.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gjenamhyq.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gsrwspypa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gjynqwqre.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gatxwzcda.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gtsekkfzf.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gtxpaqsnv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzrhdrkvk.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gaujoqyra.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjruqypbj.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gltqwwvsh.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/geflwzcbe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gimhookoy.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/glqybpbad.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/grkritsdg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gqnsjmerl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gcwteoisu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/geofixfgm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gurdxczwn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gxveqfxtk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gtszpbcxc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gkkhhlopv.sHtML


<!-- 参考信息 -->