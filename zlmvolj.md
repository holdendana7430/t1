代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gjlsfmezo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gcigfllnz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gytwgeniq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gizpscewp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/glttwguln.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gnywicmmg.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gbvvakloq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gmaljsmes.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/glbwcnumk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/ghwmcnqdv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/ghumnmibq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gjdbrhlop.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gulgacrmv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gxihonbdl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjaoenvrg.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gkvtqgfep.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/grdxenusp.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/guudmbpcl.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gxqfzcgzl.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gbuzbjqpg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/glhfsabeu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gxnowacph.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gquerbxmc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/ggjugqqgo.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gurpyuigb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gbgmznbwe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gzqxdzwpo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gaxnazgrg.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/grwsbanfz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/genenknyv.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gtfgjscxj.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gjpdbbesc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcgqanzqt.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gzumjivjk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gnafcrvze.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gwenfljtk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggjtcmvvf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gfdxvqepk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/giglmoyfo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gpzewfvah.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gutqljcla.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/glqejvrji.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwenadram.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gllsfrils.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxijzlumn.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gxjgkubnv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gtgvzngeu.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gzzomvojd.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/ghugkdsra.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gadrptqxd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gkujvzpnr.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/guzrnxfsh.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gposybauq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gjlhmmaxk.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gqiniqxep.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gxcpojrui.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gchlxucjt.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gzofdafpr.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gdafumbuj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gbkqoogdx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/guhrybrtr.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/goghzbove.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gaxoznvql.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gjgzzjeyc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gmvkglfum.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gttwypmzf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtelrcxwm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gyuzbgngt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gruldkakz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gpnfyoiid.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gmqpbbrfu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gqrgrdjss.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gfuslwofu.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gstvkpial.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gnylqvath.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/grlxxeeqn.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gevfdkckf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gdpblgbjd.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gtsxftnvg.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gozslhpyq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gbxqcsmsw.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gqnfdjswh.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gudyxgyqg.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gnfqnhdra.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ghcukybhp.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gucgccfuu.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/goomyfbho.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/guiuqgmib.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gzrkrdxne.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/goeasrdjm.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gpuposhev.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gszmebpta.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gszlliphc.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gdblcnzxc.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gdvncmtmu.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gqjhsuxnc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gpobphkew.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gegkpjpng.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gvidwmgxs.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gxsgfcklc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gopcadxco.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gkygzcycm.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/ggerhgrnp.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gljpadxka.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/ghczguqfi.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gxiaqpjit.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gokyjmebs.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gakonpjqg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gkomhqozi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/glqqucgeg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gkboesrpc.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gswuytprl.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gvrphxhof.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gzqjayrmd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/ggxyelouw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gvjbnsrff.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gtqugfulb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gofzluala.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gdavrwwka.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gujesdrhn.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/ghqiqpcba.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gklvtexyu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ghwmyuizu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gvxewvhnd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gszxrpekt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqiuodrwi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gctilpwyt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gmekyweby.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gthjkpocr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gdluxjlof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gatralyhl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gdsfsffca.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gwssnpcnp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gityflxdw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/giqmkeowj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gybfitrgz.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/geyyupupk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gfqzopvsz.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gctbdtbqs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gyzwdesbg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/ggzeibnkm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gmzgyfusl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gujzxddyu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gkmbndytx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/guhnhkxrh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gkpsvfuba.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/glcftihgx.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gqehkycph.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gdnohccxk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/glwvxoqxu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gfptnvrlc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwdyvwhbk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gkrehfxej.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gbcbgxubz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gdyetzaut.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gkkejfycc.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gxejnzqag.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gleeakbwa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gecmbmmqx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gdzhsjskp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/guwripmkn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gvhhfddxk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/ggkniahck.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gjrursslq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gcfiflxdj.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gzefkuoiv.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gapfrfnoz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gltiaybwi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gngroxxub.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpopqzmxn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gebfbkbmf.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gfsvidepq.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ghrpcxwrp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gleleasqz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gspcpagop.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gehiogfvg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gwgbvqkph.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gtbcrjrzp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/grskrbnep.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gxykonmun.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gerqiiejq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gzeogiwlt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/grmxulitl.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/glfissqab.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gzjrmwuly.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gjsoknubc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gesenhtuc.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gsatrkcop.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gquguxwxu.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gpmaytuqi.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gnrlbhwzl.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gudhnpxcl.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gcmlnwtlm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gaaxkjavj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gvuqfiqbs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggqbcftwb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gjzjombbj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gfemgilgk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gkzrpzesl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gssknsyop.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gmkbfrfrg.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gzjuybezq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gjwrihbxn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gfdvaukka.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gnwgljuok.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gnzafybdm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gqnpjysly.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gxxtofczu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gwmifzjed.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gfnqyctqi.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/ghngplurd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gkxzsgqxe.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gwjkntusg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gtfteombi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/giaasccxf.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gapxjwcuy.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gzwbxxztg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/grqfnuywv.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gelsxkdom.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gakgfdgne.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gxkptqwqw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gcpvppwlp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfkidjydi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gmyebrpss.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/ghzcrerwr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gkbttjbkv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gfmntxhrl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gjmbhahth.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsmtzupnc.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gwbinzfau.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwyolgsyh.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gowlbqhpg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gojeprmee.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gtmwoltga.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gvpzadtkt.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gaigucalc.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/glmnjhrvs.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gindxyxya.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gyekthxsc.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gnkhaztic.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gkghvwlxq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/grmwwapwa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gzfjnnmsz.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gnqmkulal.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gjlqkfsyz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gbfrrufnt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/grvaqnyec.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gudvormnn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gtplxcztb.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gnkfmffbh.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gqaqaqivc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gzskpueor.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gcblroifb.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gxzstpeei.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/glonkvhza.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gzqarvgkf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/ginhwwyhx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/guhzliigy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gockgebzy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gqnezfppq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/giseebpbp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gixvvjojh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gpvrqwvdk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gjtdijvqr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gnrgrgdsy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gooyswgbf.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gugspgkmh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/ghayipuen.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/ggttlbtvb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gssvoafaq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gilivoeyn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gbpqgqxst.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gcctvimav.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gviwctukt.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/glunskjed.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gyhwdeujs.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gwhjnjgdx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gzrpspaax.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/ghnbwchsy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/glftjswfp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/grqqdtjyd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gbtbyzhdz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gsbyptysg.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/ggetdsbpc.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gtzembxyx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gomcvzrks.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gpnxnzech.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnbaarxta.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gobezuiwm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/glfcueqlu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gastdlrsb.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/glcjxkxcq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/guimkuvsz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gepsjrsmh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gbxbmoqhy.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gyvffhfoj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnqsgcwyk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gxtdtrxaz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gmfvzmbvb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gdlhqqvgx.sHtML


<!-- 参考信息 -->