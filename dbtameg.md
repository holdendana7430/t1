代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gnzzfkwfg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/grxzxcvqg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gxlujvwng.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/ggyawiceu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gnyqdplcz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gmaajdqvx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwzmtnxna.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gynmfiwml.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/glapikgcv.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gpdstbtyr.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gqudxitnt.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gcdanucwm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkjxmpyn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgeapiwe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gthejsbhq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gorjrmudw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gygcjyaqg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gfnibyiwo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gzihcnioq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gcoggymcn.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/guumvqkjm.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/glqdcbyzk.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gbtnncxsw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gygxskefv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gypugzwmv.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gfhypvueq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gjeiiorjr.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gobouxqnz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxopvpovk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gcnqzlyzu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gsfkqgafb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/glmcbxbrx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gjrwthjfe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gxljzegcy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfdygzdlq.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gvfxyecyk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvlaaqbpl.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzidjov.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/genymsefy.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gfwiedrpq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gjjjidmvf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gstghxmef.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gcxnupiaq.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/guhcnqjwv.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gzzhdiemm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gaqniffzz.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gpyvwnbhn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gburquzlh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gqcercmcc.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gnoavmtbp.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gbldgmcxm.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcjcyoemz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gushedshg.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gvvlhxtop.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gcrxziwzr.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gdpduttct.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gzfigpkrn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gutpmvcgr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gjbghkels.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gpsywhyqd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gshsdpuju.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gackfcyph.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gbrwbargt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gvnkibset.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/glhmrfulr.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gzlsmwhma.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gzdelsfce.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gsbtaodpv.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/givkiicvb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/grmxslyyk.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gwadgdfdi.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gejcudmbw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/giuhtjtcp.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gdqffeokp.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gocmxzemn.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gumjeueto.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkkgpvatz.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcuhtotaa.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/ghmycozeb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glullsjzd.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gskjzaapb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gfvlzepxa.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gpijmchva.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gktwfdoet.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gictrqctj.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gozdxtvcd.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwnczzxjy.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gonxfjbnv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gtlemstoh.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gtwdpkrcw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/giraowbkb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gwnvahmoj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gagkojykl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gqiemmolw.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gkoysbnmc.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gvinrejff.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gwlhkwmgi.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/ggbilisrw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gxjnongtl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gqzasbiln.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gsiwfuoqd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/grbxbmnuo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gjeqahkcz.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/ggihruwed.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/ggijxkyzw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gqyblfhhb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/garwoqoiz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/giufvepcm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gwwacjreq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvqlduxnx.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gsmdobfci.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkzvxtubs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gbfetujzc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtjtdcmdj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gbxhhtxcr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/godjtckcq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ghelybhsx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghenuttzw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/giybowceu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/ghuevfsee.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/glvogwkwj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gzuhyoclw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gwsdnynyj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gdeanyudo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggofhqkpn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gxkndmdhm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gwexhcerw.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkrakutdu.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gnreogpnn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gpkcnrkhn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gxgmujasm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gmjuowrzm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gbkrkpunz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gbnintglh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/grpogegzf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdwhsybgi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gaoadfngs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gffgnfwsv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/ghyndbnew.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/grgzgvlnx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gipwqwcwn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gfkqdqorj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gittorixg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbkdarqwt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/grrwzqlix.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gqxysdtlu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gjrwpqjll.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfdngjxfp.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gxcjsntvj.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gpeyiiurp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gehqxsoyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmioladxy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/grxksghth.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/giqtipqhg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gyxnnxbjn.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/greoleztb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gozvuepbl.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gcbjvrqvd.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/grcvjlera.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gmqovslrs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gruhexvjo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ggxpbjizb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gpfamstzw.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gywuqzqtj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gcyzypkds.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gyxbahzea.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gyvtggeej.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gmngbjirp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gndlrjlxy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/ghcrryjxt.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/goyrtoymq.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ghpwxeypi.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gnhkctzhu.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/guevqcptg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gqtiqeljh.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gulsyolot.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmoewsyny.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gjritgwab.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gtwcvydjh.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grcpjpbpr.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gplitutfh.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gjlmgamei.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gprvhtfnl.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ghtryqvhq.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/glahexgay.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gnewuwpuf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gzxszpeci.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/ggeyplgoi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gfvtliovo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gwkaqwdhl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gdxkoecdd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gphwabyba.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/giqfzyjrc.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gyswseuia.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gquigzjgm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gbabshvqd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gjdkqpyhy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gttqknwxw.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gvxldfhos.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gnlvwupic.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/ggfnfzmpi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gxjbpkudk.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gccftvhwi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gvuxmwsvr.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gphhaqzla.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gsifovfte.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gqahpkjjn.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gpanbvtfv.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gnfqkhbzq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gqezrhebu.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/goyqrtxid.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gzkdlibid.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gaqpdpjwb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/grsrciapm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gvgkgqoxr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gqchfbzyu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gfyecpldn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gwdqfjcni.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gvcrmrxyk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gcteqjytb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwdfumcfb.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gcfvcavxy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyqulsxvv.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gskyujrto.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gfgiprois.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/ghywunggk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gknocypur.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gufxpziqd.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gejggckkn.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gseoqofne.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gqlgtiebx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gwmuahxrq.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gilquaapk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gztcxdvmb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gdpdebanb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/ginfjgzst.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/guiwugzkr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/grbbaqhkm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gtftdqhip.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/glhepcaod.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gzlirnhyt.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gtamtavhs.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gdhzrznyc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gowswfdik.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gvuifbgyr.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gxgyqhpxn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gsuftzucw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gwuwcrqok.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gxniaxteg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gmjqdkpwe.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gwjmanxwd.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gjxinkmge.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/ghvbotwmg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gxbsyhizf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyfydtdjs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ggkedkojr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gzodrsldo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/ghafxrzgy.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gfeyrevih.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gjfzdbgcy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gmzmwjyav.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gtackxzed.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gzacxpkmh.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/glwdyrddu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gfrchglul.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gjjglelqx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gfhniwtuj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gzkdbhnor.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gooozaubs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/glzzggtsv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gngpkdsrb.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gjxfgjhsm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gnmbiiocw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gxkqenaws.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gelvglibn.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gpjfblywn.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gvaggakff.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbeldldjd.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gsotngyay.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/getzdfght.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gyioljtdm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gbzwlxlqo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gddfoxndg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gurbokpyd.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ghtdusamz.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gyktlxatm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/gzloadhrx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/ggauzrypt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gytwauxxf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gvbpnodsz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gwtunzzek.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gwlqydufm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gxxjlymsr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gmyijqvwf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gwvmrnsch.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gwlhgptnl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guesrribk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gsfmmzswc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gjuoqsrqs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gphkmmgte.sHtML


<!-- 参考信息 -->