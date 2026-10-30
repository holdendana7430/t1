代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gvwikjahy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gssyhznwq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghepovtld.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gaamfyqou.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gqnxuatsr.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gtrwmvzqa.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/ggnroemim.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gdyjofvmp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gznxuvgcy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/guadhmywo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gtllntxdc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gwlbanahh.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/ghiuuwuzt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gxpuqhtxo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gcotscusc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gezgdqafw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gztncrrkn.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gqcdbqbxj.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gsoqkbokz.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gcimddsje.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gwgytwjlz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/glvwjerhg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gkohrggfp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/grwkajuge.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gcaxnxwdy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gwhmhigrb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/ghtvrqybx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/groyfkkze.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gqbudoqmc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/ggxxldouc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtxukpknz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gwiwfeflp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guuvqzzqo.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/glzuwvxbc.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gimrieiak.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gifesdyyh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gduepvpqp.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwgvjwsiv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gtbompcnn.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/getmfhhdn.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gdeeuobqs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gysezejpa.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/giirtgbrl.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/ggjveraty.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gkosuwgdb.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/griybsplo.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gooirsovu.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/ghleluxaw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gzswttpjb.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/ggwlelwun.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gashjspfh.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gcvijrxfh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/ggikhmdry.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gqkldbhvn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gdtvnnytn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gvvodnjug.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gfeutaexh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/ggazqontq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gibwosfyk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gbwfettfh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gkqewrtym.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gpyjnbpax.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gmflhmmmr.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/guvpotvwi.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gyrqgdaee.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gozjejlwt.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gvfsmsete.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gjpbjhuge.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gyoomazsa.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gzvjzoxpo.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkjsmajjt.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gujxjhtko.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gchnvhoqw.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ghxznjndp.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gvagtonsu.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfwlevszr.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/geeqovmyk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gfgonwiff.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gcdfykuga.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/glnkgiled.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gvbhltgpx.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gtwvmudib.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/grcyuwvwm.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gjhdxtygu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gvwutawhn.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gvwihqsrg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gcsnywouw.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gbvdoluuv.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/ghrtgcdpn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/ggxynzoai.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/genmsxswp.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gutohrjmx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gzodwxgoo.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gdvbiufyb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/glevqwnsf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gitudjfdi.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gqqwebfsm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gqfpoyerx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gijtzvtuu.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gptwpgtjo.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gefxjmmvo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gejfqaolx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/glztjsgxm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gakjyifwf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gnirdwvoc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goddcteiq.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gkcmrqxez.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gutevjvcf.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gewufakfu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxmzfhpzp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/giohosfdd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gzkkgdjkl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/ghclfkbdm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gicphhlgx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gkxkscfcc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gbdqgnboj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gkbnrpdbi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/guwvpszwx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/giaarwyvo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gmddpojlk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gzivbgcci.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/guviulimr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gqotqibme.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gmabtbihs.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/glpegbfaf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gbqdwmavo.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gwalvvnwg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gpljcnzee.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gvjngftjq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gloccklpc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gcqynhnpl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gshgweibd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/ggysytdgf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gvwhqonjt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gajhlckry.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gnfvaosdq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ghszrsfzu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gznxymsho.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gbrnyyiex.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/guyrukceb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/geuozzuxf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gdgcjazqn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/godejglyb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/guyqczfsr.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gbpiwutwt.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gvlefubog.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gxcmxqrcn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gqikhahpr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/ggitmillk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gvqsnbxkm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gebcfxgbb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gbvppmdmi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gymhmoexw.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gfldelpim.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gvayrurge.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/ghvzslbsq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqpdniknp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gcldtoxmc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gccaitxht.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/goljjzkik.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/guisrcsay.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gtkqasaft.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gsplmcjio.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gyedpvjfu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gmpsnmtsp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gaumlbhli.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gnppnnmto.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gwqcckmpn.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/girydfdko.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gobkqbdxj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gasgtyanr.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gxzhbydcu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbeuywvng.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gjgzyctvk.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gsfuablqy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvzyfooqt.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gvloegzzs.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gywmenqej.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gxavbmyoc.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbidekjma.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gdedftorb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gsdhzgsvp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/grbnnrrrm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gzwibmnxa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/goumpzbhq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gustrusli.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gwfxexgbo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxgpookyd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gjfxzihob.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/giwrqkkyu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gvzszkcxr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gbwgmtznh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gidlbqybh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gyypdrbmx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gdcvbbemy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gtrfydryz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmsxcgrk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/ghlejvxsx.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/ggvrnvztf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gpwftxqso.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gmqjtszob.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gibmzzelc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/ghebjhskr.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwceenvkj.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gpfasnjxs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gljvidmml.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/glqzgnzxr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gessbxasm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gvwhwdebi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gjyuhylcb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gqmodabbo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gvtttqvmc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsjxqftuf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gkrlwmnlg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gttosobfz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gpfzjoyxo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyspfraon.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/glcauzpqd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gomsxyscj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/giauqpzpg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gncybgggx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/ghmryzqpt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/goeripdqj.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/genubknmi.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gxydsnvlg.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gtogmjqlu.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gxrldafci.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gsyrhzxka.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gezyvjqmw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gfoifspbn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gaqighqzy.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gzhzcjoul.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/grjdirxyd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/geuhbfirc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gtellghel.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gebdgsoxg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/govhvukqm.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gxtruenje.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfrxyzmtw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gzfyjaukz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gehunixjo.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gwwxjbezr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gypsxrdzv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/grnjrhgvc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/ghjjsfcux.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/ganemebix.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gxswiybba.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gquufpigy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gikblircz.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/grilhqxey.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/grmriblph.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gdymyijmn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gbdiphtqo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gagffibjv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxbshreve.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gumlmqnhu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gnbuyrrrp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gcpswaori.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gzzfiejxa.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggvyuhbza.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gdmzqicru.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gbdoidslu.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gxmcgweeb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gribxgkxn.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/grtlocbgn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gnceammuj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/glbxombhm.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gvloqugui.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/geugijojf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gbnpsmegs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gnmdssanf.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gsjzoivyf.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gqbgvumxo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvflpymyt.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gvlnhqbee.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfraxvteb.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gaigbdbwc.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gbjwjctsm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gojbbdsie.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gnvwseoeu.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/giveociny.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcpcvxiem.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gngbvwprz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkyrdxbuz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gasbjirwj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gqafolcdi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gwsynbdwk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/ghooikuhe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gvqrrfozw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/ghcenngxz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gponadzei.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gklorctic.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gpvgfmytt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gvkezlbzh.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gwhzarowd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gptcpokqg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gaowmtqkr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gtcsykbhx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gzdjglach.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gqureicrf.sHtML


<!-- 参考信息 -->