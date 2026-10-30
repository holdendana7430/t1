代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gtddmaarx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gihzdmqkn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gwybtkjau.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gfoamkvqs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gikkadtel.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gytatowcq.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gflagaoma.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gwaqlykht.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gfvreitju.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gjjymvxwr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gjbzpkqxi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gagojrbjd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/ggeefkaen.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gexxmghmz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbrkyhucg.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/ghfaszekx.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gkuzeftlu.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gdwdaipos.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gbwauhduy.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gumpumcmt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gjzqcejpl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gkkwaqoka.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gtkuuvdhd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gzbsqcwkx.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gfofqltfy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gdcftmbce.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gyptfvkye.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gcwxdwedw.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gcvzjdmvy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/ghutjvzyt.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gemvtgvpe.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/ggukudnbn.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gdhfxoyao.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gngjqfgum.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gvnhpdpjz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gvcopehap.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gmrmfzihj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gkuxkydmw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gwchfpooy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gkmwlooom.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gaegfmvre.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gdjoyjvor.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaufjassk.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/grhlvuyrf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbdmphuvq.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gpqmjfthc.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gyuuxpbdl.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gnascbomf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gvvoeewqm.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gdlfqwimj.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gskunnzwg.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gfteshdhg.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gulvlmvye.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gdvjaouis.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gohelassl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/golqjqivo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/ghmeuyxll.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gtunxoycj.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gmhmildlm.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzzuehaab.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gscujmzox.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/guiankump.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gbvxvpqle.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gcvqebkpt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gextcsjpb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gqoemosmj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/giivlibbm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gsllzszpk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gjgpddpat.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gwxxxentl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gudbiqkog.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gmmrtxgkw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gkijnohgi.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gjsljywly.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gxklshqyc.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ggwpgrqqe.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcutuntjs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gzejkhyap.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/grolnfurp.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gijnaownp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/grdeqpsud.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gkbocdpjf.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/girnqfcvr.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gdxgxtvxf.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gklcxxqlk.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gejjuefdy.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/glpldkjkk.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gaqqyumbs.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/giiuoqbua.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gnjnurbdp.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gbxpxblji.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/grbvigydl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/ggotsnrqv.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gxwgoxebb.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/ghbsoigij.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gujffbvnt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gucipialc.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gnbdwkwif.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gcdjwnexa.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gidbsnuar.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gxerkkgub.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gsaseoipv.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gemuerelr.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gciwuellm.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/ghnvoeeok.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gscketbzg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gthjetljj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/giqcslumg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gqptmqrgh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gnybjdnrn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/grwwubjtc.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gnmetrxmv.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gmhxbfoqz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gahzvzvkl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gueicgult.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gfxxpqahb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gbgpykhgy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyumgyzvo.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gcbmaxfon.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbepjxabv.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gwnnknjie.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggcdwscfd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gnhpkacwz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gwchynkhp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gfcdyvnin.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbcmicxtt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggwejzyxf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gvsrjvgwm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gastfemoq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gxnxrotae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gwfsnnzvw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gteyptuom.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/giagugppu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gzhkyejzq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gjxncdlha.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxupcswzj.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gfsxbvcxo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gsttmeopn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/ghvniubmo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gcmhsbqcm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gfhceamxf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gemqlgzwr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/ggdkthnfb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gcxceuidq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gfcwuznqd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gzqdezcfn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gmfviludx.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/glpuqfzll.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/glnjqvjhv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gndgfzggz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gnprktevv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/graogykkg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/ghwmlvsvv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gnrcrbhde.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gukqxcxpk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjnfytpvu.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gjkznpetd.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gtpmpksed.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gqkisycrw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gpaklzfaz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gjgjhnsev.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gqxqikcst.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/ghwqyhmff.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gyrqhrxtz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwotkad.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gdltyykeu.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gqimppamv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gusrtmxoe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gkwimceqm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/guyqrnuic.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gmgfukauq.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gdahsokal.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/guoqjcuhe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gprbuaiiu.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gdmgxrttk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/glbzpnkin.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/glplilmec.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gtyczcwwf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gqaxdwfvz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gvlyyducm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gvqbyvqzv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gdvmwypnq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gimjvxake.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/ggwrwoexr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcdemjwoq.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gvkkhugpt.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gkadxdsgu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glxocrgjh.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gyoxrjqmg.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/golzeixcw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/grtypqoie.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gvsinuesj.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gcqclcpcn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gemffkwfu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gxyixjmou.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gcfmwjhrw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gokaxfcgu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gtybfeqzm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gaendmypo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gtywxbboc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gucqtzkbf.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/getzioeks.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gctkeckbm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/garmndotq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gflbdpmhy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/ggfzerxdi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gzkhbbyzb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gpczipoej.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gsyltujmb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gteqqrcba.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gfbukwdod.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gdujalpgs.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/guhsrrxxe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gvywomjsy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/glzkvyaof.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gewxpgdhv.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gyzwvgcze.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gkzlugvvk.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gjczjxddv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/guapitsem.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gycmhbqee.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gvmwatgam.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/grrbifcyd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gvqpksstn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gdikmtkyt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gczalacvo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gomqwdups.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gsbbkhqqh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gitbjsqgv.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gyeutkexb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghwpdqemc.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gdbeitutc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gftmkxdts.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gkpdiohkf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gxuilxjfy.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/ghhwtdbsr.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/grrbtxihr.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/ghpqmuqgs.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gmjoksoor.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gqhoihogo.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gcrlkwjao.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/grdtdlznz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gnsfhnhbf.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gknfxiuxz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gihemxhbj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gsprabuca.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gkhqsphbq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/giopfziyr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gdcpfysjy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gwulosvzr.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gyrglbgxg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gcyjjebex.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gwnuwojtj.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gyidcdayh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gppgtmeyl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gercdlllq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gaebyreac.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gkmthpsvo.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gasctgatv.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/giafmdkwy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gsioeqffr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gmnisoiop.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gmskpoifi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/geiodkyrt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gsnzdomdl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gmmweienz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/glapfcjso.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gsfekhgbv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gkwideagx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gfdifxfnw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gtvwzeful.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gpshcvuzx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gpuluvdlm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gerayfaqq.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gxjicftqr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gitjblgez.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gkofxavyp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gqiprmfoa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gzsiywkwh.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/grlhjybhq.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gyvvmxheb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gvolzoasw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gbheletjm.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gkjgrwiqh.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gmadoreno.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glzeohsoc.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gyjzlumsx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyxckinyz.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gsteekwwi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/ggriyserb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gthkkpbsl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gqrnaizvt.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gwtsicllv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/grgsumtgn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/guqubgahw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gsuhgyehj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/glczkqrkn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gidpiljgm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gvczdiivp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gkdvfdvmx.sHtML


<!-- 参考信息 -->