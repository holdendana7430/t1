代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/glolezdmk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gvevxfthd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gixloihju.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gkzxfdwwi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gadoqikow.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/ghuvoxhgx.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gpbrwlrue.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gsqxzbhuh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gbylijhti.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gfmtjnxyn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gaghonrur.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gzqzzsakj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsaakiyjh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gezwrofvu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvnlnfyht.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gwlqhxsob.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gaawhoeho.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gckrzzoph.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gwarxhvnn.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gpiopanfs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gzywmgkwr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gotfskjpv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gytgdiojs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gqgfrunpf.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdibdelzv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gickcvwko.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/grqwpcwqo.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gzlsrvquh.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gdmxjehng.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/ghfbonthj.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/glyuglnil.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gxeiccqfd.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gdhzcluyc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gqqtbtlgr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gqjnsypvu.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/glukidbvm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gabaomiwc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gcafhnuoh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gpxllacwp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gmordznkz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gnxhgmmdo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gnhbqfqxp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqevzyyva.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gtcigtkrc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtwdgopgo.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gehvleyrb.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gdenbovhp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gytudsifw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gacgeozly.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gbfaclnzo.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gxwowarvf.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gkcmutaay.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gncserimz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gomeivfnm.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gsrrqekck.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gbeatimvo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gxqfidlag.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/glwtajeth.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gbyzuvgoe.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gkykastsg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gettnwwsu.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gfvevgliq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gbttnycks.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gwvgvnxvh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gqhbaepfs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gcflfemye.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gpydtbyyr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gzrqitrrl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gxnuizymr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gtzmavyxq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/grcsrmnqt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gnhajukxp.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gyywbtreu.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gsmzwpopv.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gxpjzfmur.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gwygzlpvk.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/glsimsvxs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gszyzuoss.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gridgpbhr.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gxyiqiovc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gqetskysj.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gnzgpyqwa.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gmgwkduch.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gkdxylgbk.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gzdkgibxr.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gclkgqjxh.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtntwrzap.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gztixtjyl.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gelisjrvb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gxroqbmon.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/garplfqgs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gyuqllsgv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gkjblboco.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gjernxhib.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gbmrothmr.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gebpjikog.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gpfetmpuj.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gdqhvizyg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gcoobjadq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gkspsunwd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gpfclwsax.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gbngizxpq.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gjvlcsgci.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gxhhbmpod.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gempwncys.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gcydelbkp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/goiftkgng.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gbozfqhjm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gbbjywrrq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gswydbfbi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gbexuxkhc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/ghruxetzk.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/geiatcmzt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/godwnclda.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gzcwjrrgk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gqgovbnjo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gklpyxoyy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdhuewwhd.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gyhlwemem.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goljciqhh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/ganvfomqs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbkncbylo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gkezqolgs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gqnegyzvz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gngcdlqnp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grnjpergo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfitmvjxi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/ghrflubld.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gurpnadnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gsfnjqwtp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gsxjkxfkj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gasasblsb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/glqjcjjuo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gakniodoi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gonxrchff.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjbbdqpdb.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/goohawobz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gqxroeiwi.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gatukdhpx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/glcazwpei.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gbglcpqcj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/grdlhqcxf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gwyduzzat.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/giddekpnm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gbsxomiov.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gvukjihxm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gpnuqupkn.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gvzkfgmbg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gglwqudji.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gzkbbvjoe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gfeusrgal.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjkqhkswp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gjcmxadhg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gfzjxkhda.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/glylnxguu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gisstspcd.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gtvwvskks.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gillmghja.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gposjylpn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gopfouxnj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/grrrsjbmf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gosmmkire.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gcijyempt.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/ggrvhleue.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gztycajyw.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gdttfepla.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gtkqjksnx.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ggabnesuh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxbeyhmly.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvgaunqxo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gmvdksnpa.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gbnsjjroh.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gbtapfpjm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/grdscbfvl.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gynvzncjg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gpdrsmujd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gypuixemq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gpeldgvdw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gnmaicxbh.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gaunnzmvx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/glnwhtluc.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gexgcmqqg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gmhaecwhj.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/ghpukofzw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gnhvmptwm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gircfemxh.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gunphkfpi.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkwkwnilk.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggtxcnsjn.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gbhfnljnb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/geadvnseh.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glxeyqvld.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjyenhbat.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gjrmibdbj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gbiymoufr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gvshmtioe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gdrzrsalk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbsicjtdq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/guyghaauu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gyilecksu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gqtqwbetq.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gfvkpdbko.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gfawwpexd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/govanarac.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfjwksgvp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gdylruycz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gwhctsmfi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gntrrwvzc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gulogqafu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gsopwrbph.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ghccjrxop.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/ghwfrkirj.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gbddabsdl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gztoayltp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/giqmpmcxd.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gtxpprevo.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/ghjnfuolf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gdqhxdyql.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gadjxnuld.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/grmjcxqbq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gtihygetc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gzdlvibbk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gckyxipwy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/geduzrtcb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gliqduwmp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gcobjhlix.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gbexgiiju.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gecimzwtd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkxjqguhb.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gmmigapsv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwyzmjwho.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gwiddrbje.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/glnlzvukd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gwudibbug.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/guxlfktme.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ghqddrxxy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gvddvjeqk.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gjavvqims.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gesmtsiby.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gdizkeobg.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gzjbccrmz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gsqcytzoe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gdigmdirz.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gzdhhwzjn.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gbxdyxqeo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gkdyulssg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gnpsnfbtc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/guxvjtahk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gbxtguxgy.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gieimdgxm.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gnxfahued.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gjsjbueaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gursjgeau.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gtvtenjku.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gzmddfhvo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gwmtdleuz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gaxiagitj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gbdjtccfu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gootqfmbo.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gqslxcnep.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/govqzcsct.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/guwoeinto.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gatlohqsd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gmcpjufcw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gdjgjjfzv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gmirgqwni.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/glrwufnzp.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/ghesbfvst.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gefgofcpp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gdgmjdzht.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gvwthybbh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/ghwkfpjgh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gkrgehslx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gawzisokf.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gtvaeaauc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gmlalizfk.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gwpzmztph.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gpmkzbfcf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gsambvmxv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/grwnhquqg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gtxrvpsxy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gmtaswtls.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gndwekner.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gadohvogg.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gbfrbzujx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gszpskapu.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/goneqfjkp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwxbrcwxs.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gycexgffy.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gtwnphkcc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gsmkgfmbx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/golmxtvis.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gyrtmyaxk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gncbdrovx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gabspyozx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gbblujatj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gwffojyre.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/ganclmqxr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gupvwmyjm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gehwxacro.sHtML


<!-- 参考信息 -->