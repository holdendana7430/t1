代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcclyjsp.sHtML

[L04] 设置超时
来源：http://read.share.fanxiaobao.xyz/Article/details/gecwasmds.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fanxiaobao.xyz/Article/details/grolsizsy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyokuehy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gddyzljhb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/glhtzgfit.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/guavfmevl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmicfsdbm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/ggulnxzwc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gclmnewne.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fanxiaobao.xyz/Article/details/gpkpmybpv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fanxiaobao.xyz/Article/details/gqljkmhkv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdzzbvam.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/geuunywfp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gntrintgf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fanxiaobao.xyz/Article/details/grgyqwyuz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjoeqsjc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fanxiaobao.xyz/Article/details/gadezyfil.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexktftem.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gwfnxbhsa.sHtML

Py:   resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gksrzpydk.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwcmlcfa.sHtML

JS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghttqutct.sHtML

TS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/glcrpnbvl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/geagvydei.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fanxiaobao.xyz/Article/details/gsztvuxgn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnskbozoh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gamdsbylf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujxbdbey.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcoycoml.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fanxiaobao.xyz/Article/details/ggwyitwav.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gdfngyhlu.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/grvtgabcs.sHtML

Java: resp.statusCode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gctsaxhgn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvadlcttd.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjasvcvx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gubcysybg.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzhelsmo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjspalkl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuhnmbzf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdpcybek.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktxpvski.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fanxiaobao.xyz/Article/details/gunjrojdb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fanxiaobao.xyz/Article/details/guphedyfn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/giizztfou.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvdymksr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwbdcgajr.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gizxntebn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjahtrlbu.sHtML

[M01] 读取命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmfsmpjya.sHtML

Py:   sys.argv[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gmlbcieau.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fanxiaobao.xyz/Article/details/gfprppefs.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtffbett.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gcgyqbhwu.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gdkgpmtrn.sHtML

Go:   os.Args[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/guwhqprrn.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrjtgpns.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gwvhnkiyz.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaahvgcag.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwprwtros.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjrdmckt.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzymvhlgg.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmyspifg.sHtML

Java: System.getenv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gyigkiakq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfkfbsep.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gxskdqhqz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvcntgth.sHtML

[M03] 执行外部命令
来源：http://blog.fanxiaobao.xyz/Article/details/geoxuxzlw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gqieapfed.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjccenkrz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/guvtxkyqu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnzsmteg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzolkcpcm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrndibvd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpeoopks.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/gibmlafne.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjhvsrez.sHtML

Py:   os.getcwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlcggwkf.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gswhhqtzq.sHtML

JS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gljtubkce.sHtML

TS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcptwquxk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsthohbll.sHtML

Go:   os.Getwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgkepjjc.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzpwwgom.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqvghfje.sHtML

[M05] 设置退出码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvwohkqh.sHtML

Py:   sys.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjavwopd.sHtML

PHP:  exit(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuortowo.sHtML

JS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyamcfkp.sHtML

TS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghatnaocl.sHtML

Java: System.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbqgnzcbb.sHtML

Go:   os.Exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzeurwlk.sHtML

Ruby: exit 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtzgsdzo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqvpndcy.sHtML

[M06] 向标准错误输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gskwjdjie.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gznkidorm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/godipoowc.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gptqwfvtr.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/ggtqyiuqn.sHtML

Java: System.err.println("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gutulvwcm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gzpyuztur.sHtML

Ruby: warn "err"
来源：http://wap.fanxiaobao.xyz/Article/details/gssjjnsiv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtibuxfar.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/gexrrhmha.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fanxiaobao.xyz/Article/details/giutvjvvx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gejsrotew.sHtML

JS:   require.main === module
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwzlxutm.sHtML

TS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuoizrdu.sHtML

Java: public static void main(String[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gpeypemjg.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjvrbqqq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fanxiaobao.xyz/Article/details/gdcloeqja.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/ggksvvlpe.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fanxiaobao.xyz/Article/details/ghhmzsvme.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fanxiaobao.xyz/Article/details/gqgawjrsm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gydvzcvjp.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfljaswtg.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gwljtqmgf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/gamokylaf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fanxiaobao.xyz/Article/details/geejjyqdl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fanxiaobao.xyz/Article/details/gskewhige.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/gjbwzlczf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxjdhtb.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/gzjequsvw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glmmgyjfh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gtrpgcpfu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgonfvzn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpksrxrlz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhetpwxo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gblppzfah.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdbkyswh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkuujjvo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceuaqqng.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/glfsrbafe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqifaffj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gmibfdsvh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrduhmda.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaeyxeti.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbolllbiw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgusknzu.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpzqfkxd.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjuacwio.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gssfcjisu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gnwlywtmq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuhpeggk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiwtagsx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gufkagnmo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gfogtlvfp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gmlmtbnmo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbsqhcjh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gafexnwrb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbxbsavm.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstftbxrf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gijpwhvzr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gahxjvqnw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ghnhjbvbf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/glrnnmegy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxxolnuk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gsbkubvib.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfhvlhlpq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyafufipp.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmhhhawp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/goayoobkw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgqmwlyd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpnzzerg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gultvuisl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fanxiaobao.xyz/Article/details/gccfykmts.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgiuzgfm.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gunjqqjcm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govtjepdj.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghqvntaws.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwagbuih.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnxocldo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtumlsss.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyruxtvzb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/gdpyzhsip.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fanxiaobao.xyz/Article/details/grttvrxfd.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gopljijko.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/geapbxddp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghqwvvh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnirumrfi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhdkkpur.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/gngyhvbpu.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fanxiaobao.xyz/Article/details/gggyqlzbk.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzyvxres.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fanxiaobao.xyz/Article/details/glkvobezj.sHtML

Ruby: // 手写 Hash
来源：http://blog.fanxiaobao.xyz/Article/details/gzonolgtd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fanxiaobao.xyz/Article/details/grjhthqhh.sHtML

[N08] 生成全排列
来源：http://wap.fanxiaobao.xyz/Article/details/glarjjwjb.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gcxemhnds.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbldvfgn.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gindkgwlu.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtchdlmvq.sHtML

Java: // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gaezdrdes.sHtML

Go:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gmrmupzja.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjjnmjou.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/grafarptd.sHtML

[N09] 栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtcrpldp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gifapwryz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gaguklkuw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gcnajyjvu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyrtpdhf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/glwmhbjwc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfqgvfpp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gtenmemkg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/geqffbtka.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/goefvnwuy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fanxiaobao.xyz/Article/details/geslutxnh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guyqprnjp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsdfxwpv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gsacqifgw.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiumpdcv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fanxiaobao.xyz/Article/details/gjfkgggkw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/guoukiagl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gussraosk.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtterjbu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fanxiaobao.xyz/Article/details/gejnnijcf.sHtML

PHP:  // 手写递归函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzwuwhgln.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/gqfkemtsh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gpkdqfbkf.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkvxkxkq.sHtML

Go:   // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvhzwswn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gelbetpqz.sHtML

C#:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/glkykfhmc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fanxiaobao.xyz/Article/details/gwiegrgph.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fanxiaobao.xyz/Article/details/ggkmnwkjk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcegvyrqu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gnznvypxl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbdgwagy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gxogcfhnp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbdwyzplu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgbwqgky.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gquaisryd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntlnprid.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwnhicfy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grerxdxez.sHtML

[O01] 启动一个线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiayfviz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gkfzchfmn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzebjltcs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fanxiaobao.xyz/Article/details/gopvbtppx.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrsemaqp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqxnvwcw.sHtML

Go:   go f()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevwzcmyq.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgxikzjk.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/grmdbbhbh.sHtML

[O02] 使用线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkdzcmap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fanxiaobao.xyz/Article/details/gfurjrkty.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/gssfcffom.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gssosoqyn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gxxgwovke.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphwjrztk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fanxiaobao.xyz/Article/details/gcfrkbhfr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwbdpces.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fanxiaobao.xyz/Article/details/gxsjzmuay.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumttskgp.sHtML

Py:   with lock: shared += 1
来源：http://blog.fanxiaobao.xyz/Article/details/ghjfsyaxr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuiczczl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmjripiy.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzeiwgvy.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfllsrdvo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fanxiaobao.xyz/Article/details/gclynfibl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuroygud.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gujkloujy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxeosbpj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupsojcqa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gawbgoygl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/grmptswes.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcqprjtw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdsqmywt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhyxffgm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtazepun.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gymnjwits.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefbxdqhv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwtgfpwe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhcdopep.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/glddfhhoo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogxojqdk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsttolipc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmndrlaqc.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfburmbbc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsyxgkurn.sHtML

[O06] 使用进程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzqolxvd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/getnqngda.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fanxiaobao.xyz/Article/details/guhsyjyph.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnitfsff.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaygentk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqqivvjx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fanxiaobao.xyz/Article/details/gntwhqfvg.sHtML

Ruby: // fork 块
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtpymojm.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gatvhuxpe.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcmnpzml.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfyltyplm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gljxhtsfw.sHtML

[P01] 生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjhpobdv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/ghupserlh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gtncqfunk.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnspmyoa.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gihxpqxpi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gaigjjpsm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvkjfvjg.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gdfkhrvjn.sHtML


<!-- 参考信息 -->