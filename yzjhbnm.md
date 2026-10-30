代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gqgcspsdd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gzivajkhk.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gpswpopix.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gddedbzjv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gbzrzbuzj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gwidljuhv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gtptfwbch.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gxsihnhag.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gkdwmijci.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gtuatjmbw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glxbvahhl.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gmuxahccj.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gvxdxrvhi.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gbplpmjlp.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/ggkliiffm.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjwdxojjo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gotmlrzeo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gfhwvusaf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gdygatcrl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gtysvjfnk.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gfldhmllg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gloflbhhz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gckqkcvkb.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gzzcdbaiw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gtojtixcn.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gfvgrnsot.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gtfzdbaox.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gvueyfxqu.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gzziboipn.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gfknncqlk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gjuywizbt.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gtgnrswof.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gmoikrxvk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gucoiione.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/guwqnxqdp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gdeizrzat.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gwoxyemrf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gaoakbxzb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqdyuqxse.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gotwxyulg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmoxllnso.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gdlzgrxww.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/growmynbw.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gtmnmslil.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/ganlnrdrb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzvqjdrn.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gszvbcqgp.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gqdzxjdmy.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/giplghrng.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gffcjcshr.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/ggoklmekd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/ggdkivplt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ghihlfqot.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/ghjtdtmtc.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gzsqbracz.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gnvtfmeyf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqyshhoxq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/goeluowyz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gycjvkpdm.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/goroqwjai.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gctpcszlm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gsnqmsodg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gerqkmzze.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gcuvxfjqt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gkxrhmgvi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gfuylgrsw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gbtfrmmym.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gcyqmumom.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gwlnlymmh.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gxuaearfw.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gdmstphhz.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gpemzlfsb.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/ghgqljxvd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gyudwcfqr.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gfxsjzjoy.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gdfcgarjs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gakskfmvh.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gziwsaouq.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/ghxkghblg.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gqvssadaz.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfjyjuykq.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxbutymbp.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/grqpbjnux.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkvaskrvz.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gzjfzxndt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gavoxyrnd.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gxbqexrvu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gfutdpzzx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gfzzpttsb.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gszakcjxm.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gfoxmyfii.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gqiurwobh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gweniocgv.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gybxaqzxt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gqcbyzyct.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/ggsjzqmzo.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gxfrarjft.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gcsxmdady.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/getvjvrtc.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gpznmebnq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gfdtnxkle.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gfacxgmpc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gtnmzxdiw.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/geyevjesk.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gcbzvajwo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gzbfatrkt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gnxfqvnfe.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/glzbsngin.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gxjqzatyr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gxxxonmbz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gegejrmhn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gwigilbeg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/ggxbllnka.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghkgsifcq.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/ghxmznjlh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gynyvklgw.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gghptxzih.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggubzynsw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gdshewyye.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gqmuaswwk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gnqsimiez.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gibqlcmca.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gquggnwhb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/grjtyuujp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkjjfflgq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gjbvyzrhy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gqryfyfwj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gqjblwbqi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gouzehzer.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gtyoifvov.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/giyzoillk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpmaoansy.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gjpcrblbi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gtnbhmquj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gxedvjeun.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gbyaafzcr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gcwlxuiso.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gzbftoamx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gbjeqobsh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gyxsvlxta.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gzjvaqvyr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gouuvxrog.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/ggluxtihy.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gqkokqizf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gksnyvrdy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/grvsrzzxm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gubchzlbu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gbwgrdsau.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gzkhxuajj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/glcjjtkbq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gczbumbka.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gqaqwkuhu.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gsrumfzvf.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqyexmtdk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/ghwbpaloc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/guzitsiry.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gxlsecmib.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gpigzbfzn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gqocgyszh.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gblvjxwnz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gufpqfpis.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gzpyoxwru.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gvcedrdny.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ggfwfkfex.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfdfqfzlu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/golhpnhlx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gppkegbrb.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/ggcfpksha.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gyvqipjev.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gfklikfdf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gaithsxzj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gncamysei.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gqkspbzmc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gnfrryvlz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gvboocwao.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gcopgyvbb.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gdjaqlaoa.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gbsvetrsd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gtrjfeuus.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/girblqirs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gbttzljsv.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gptruutia.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/getfotvvg.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gaategatw.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/guuklioef.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gyxyfjtpj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/glzdilnwe.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gzlcxomzz.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gfhtdmcpx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gompagnrv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gllfqbkle.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/goqzanago.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gklxdhlbg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gefjpdzue.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/guvbarjvw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gtgexoryb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gkcmwfjfe.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/groqfbiqf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/guxuvgmll.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gbhtidufl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gbzqlatvq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gmpowypld.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gmvthrhpj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gqdhhbijy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/ghfpglzai.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/guicxzchu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/guhiwadki.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/grlwkjjvc.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gzjffbqlq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gsmomfgnv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gnunyxspw.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gjigbcatx.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gjvdlrklu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gguylrjje.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjnigwxqh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gqpcwjrdp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gzehlxrke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/ggnlmaqhb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gphzxzlde.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gknfidxsg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ghmretghc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gzrhtafqa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gyzhfmioc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/guhqqbgtv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxhalrmso.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gxpvyqkll.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjbxdmhtr.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/guylbnkej.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/goynvfxpg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gafiqpvrq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gizkgkwxy.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gptqljwcc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gnxcvmpdz.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gjxrdvqnw.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gnilcgaph.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gllgctyqs.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/ghwqwshst.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gqtiilfvi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/ggjoyvmxl.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/ggrdbojtl.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gwfrfuswk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gidlccuie.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gzzkybdrg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gfaeslxhh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gjivisdou.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/ggkzyotnm.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gqveniggl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gxvrofexy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gghftspcj.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gcmtvxpgb.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/glmteyifa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gzszzhkyz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gcmkwuczy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/getnsqnbt.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gnzmonskg.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gtrgyyxoh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gekxvdpfo.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gjeupegtv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gxfkhcdex.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/grdasjbst.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/grmkfibwj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gfxvpjfcu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gwlewcsgp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gnsaqjusq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gjjuvxcsx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gsgwascyt.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gtobyzqcn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gzdajeiuw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gqynnmbpc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/giqexkmyd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gommczequ.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gyghswquo.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gfhbxprhq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gcnfkolez.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gndyounfh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/guzpxvxrz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/govyugxle.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gxdqepyqm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gfncclmgu.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gebvvovsg.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gziokhwyz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtqalrfoz.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gvuwqyxrx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdafphzmx.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/glftpvnsn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gsuluqqow.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gdizskqas.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gkkbvpwar.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gmdhnapsb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/genfwuoyy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/ghmojzadh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gqtmsfztv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gvomildpj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gpghsfeay.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gjtucijku.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gnikkftek.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gmculxqzs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gsomegpvf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gmplmrtsn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gagkudbms.sHtML


<!-- 参考信息 -->