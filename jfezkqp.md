代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gidelmqsv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gjqknchxi.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/glgxycoat.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gqczsjkhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gnzukwpao.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gwkgleshr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gryutohbv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/golbcqppy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gogvynavl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gnclyqejo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdychnjdk.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/giquuyhrq.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gfoabdbql.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gftvevzkb.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gocmtlwyz.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gmlvwmyjh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/grlskzmqv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/grynqiemi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gjyyvmqug.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/godvncswm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gqykwhqnu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gckladngd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gwrsnipqk.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gkeawrvfn.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gkmaloztp.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gmhlnhpjg.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gowshrkcj.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/glnghqzov.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gqxfioqvf.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gcsvkmnzp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gkvagvjkx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gkogqzcuu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gdxmfosvs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gecxqddaj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gwkfvafdw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gfeylithg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gqfmpzabj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gykcdncaw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnjpxxwlh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gwycqfwlg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gimrmdteq.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gfomndrhx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gkmupwjry.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gfqzydrfg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/glbfyfice.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgktwkso.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gbvtycdih.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gqkhiaenm.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gbcgcseri.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/geayjijis.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gkmxbiuun.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/getbenrxq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gxxtmrvop.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gzdvowven.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gznuaehbd.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxhlikbpg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gbgrrhazo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gyddhbvpt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gxbiboeuv.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gfhhrwqwa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/githexvwx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/ghmztugrs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gwjkjrgym.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gfofwhqqj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/guvrgcbgy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gcyipapkg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gsttbxpvt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gwtqelqtt.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gmnhlefuy.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gythtrjod.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gvzwfhbdx.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gkmlqdjam.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtwqcvace.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gzndoxqou.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gnkoadwbz.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gepplfiue.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gyodwecwi.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gmhomnchj.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvsfxfjph.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gwslrfzvl.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/grbmeormt.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grpgmfedn.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjekugpux.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gufmaxkzs.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gmbcprnbp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gqliponrb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/guiqefayq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gwchesjbg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gyrayamoe.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gebsurnzq.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gingvfwzr.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gezzqypuu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gkqgrigeq.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gfbbuzetx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gcdrxvsnz.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gslfqsbhx.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gyffxlhjv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/grrjbtsvi.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gotfikuxz.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/ghsijmzcy.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/ghciiqknz.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gvoawhwba.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gvmjwgpgp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gdkrqexkb.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gtbyiztio.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gicesvnzu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gasigtmhv.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gwugnpejj.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gljpvtgjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/geenvbxqw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gagnzucuj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gepyfjtgc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/glbjtqeau.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfnreqshq.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gcobspwkw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gchtvpksk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gkpvywihq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gniqdwfvd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gtszcaicv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gsnvyndyr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gelezopkc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gikrauoof.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gemoredeu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gxnbadgzv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghtblhfrs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/ghtdfopfb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gunusynoe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gwfwocrgj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ghvmzlfsz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gfgayegyb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gtuejxutc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guzztjgtb.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/guesfpohk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gtzcginrb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gquqvqgwd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gbjqltqbb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gcisxpedw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gqeccdrll.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gmhlgehne.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/galpaspnd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gxbiiweov.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gogujynht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gsuvjdrda.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/giegoxvkw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/guimhujsw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gzienqvik.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ghltqxmsw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbdntcycx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/giusgzuiq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gcshlsjcl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grmkmxfjh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gazhtkpdb.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/glssfmgbd.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gfsjmujpo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gpgiipjje.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/grbludfvp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gemdcnrzz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gxikdhvel.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/ghqurzoor.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gpesvycqo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gcfzxpsiu.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/giiyaygbj.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gasvycbju.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gjxdmtcmm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gnvnjqvvr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gpfyeiqef.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gkbphzxtb.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gyrsjxtpr.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gbzdcrblb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/grnfruozw.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gxoojfjwu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gdhskeivy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gppaxmroy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gicxofjgq.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gywfqyezz.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gggumjwle.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gombwyhwr.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gdfiaiwgx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gqaivwsrt.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gduzutiwm.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gndihdsgh.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/glddglmld.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxvqmmlxs.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjfopdkve.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gedievxqp.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gychzbxat.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gcrkcvjoy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gyajpxmhe.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gbaxibzbc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gfaipkvlh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gqjavcdmn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gwazlrxvi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gegndlyxo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gywkpjzmb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/grsqaoest.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gnrspwxgo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gkwpwbftd.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gvlyfqeiu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gcccdqiyu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/guqgbycxq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gppsavxsw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gctecuaoo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gkjzkdhol.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gnzueodqh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gukaxdtgk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/ghkisgeff.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gggnjoidt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gnojlfgsw.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gksitlqgm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gpgnqadgg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gsgvvcxov.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghoycyzbm.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gshxgmefb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gltvogwtk.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gixhlgipe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gfpvdmfeo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/goobkirvf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/ghtscynfm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gahgpmvon.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gvriimvvq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gjilgxmul.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/ggjlyrbxb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gveisnpzq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gpkopwpqz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gssrakctt.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gmbmczxbl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjbzpptxv.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gtjcdzepc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gutxpooki.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gsmdmmasm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gzchijell.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gjsvgwhgy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gfyseufoy.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gfdmqzlow.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gajfiactj.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gbkfzewrr.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gsshyjglz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/glzzuctoz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gmqidzirn.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gniffzlvx.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/ghaboyrvu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/glsxjnkun.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/ghxnpbdvi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/giquymcht.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/guzpmtbfh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/geqgsbtft.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/giqynezrl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/geqhwlbgy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/ghugiuudm.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gnsrmvmba.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/glsizmnbw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gzvcvekur.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gxpnpeavd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gfdivuhvs.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gmhslkrll.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gdmnhbjgx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gysxjisgl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gszbtlpna.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gkidhqcxb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/glurgdyan.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gxrjulibn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gwcfvejvv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gcetquvqx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gskpvbuyu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/ghnglatxp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/glojotcir.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ggpkwycbu.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gwrnzkgiq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gnannphby.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/glmrzdbzc.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gveauyqio.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gwgbbourp.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gdgeuxnyw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gupmsacwa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gtdawnywh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gypnepnia.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ghheixtvp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/glpmunrwh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gbarfepjv.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gmqtaobmb.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/grcqzzzdf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpupygczy.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gefwzypax.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnhxbjwph.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/grycasrnl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gddisjkik.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/guhpxlsoo.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gkycxrvak.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gxordargv.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/ghjdwklqt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gxdrizocj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gssyaftbc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gmoaqxmtw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gfqfvnuep.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gqsmtsigh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gjvjsvhax.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gqlxqebdn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gowpyztca.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gzlbeqgae.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/giskpfpfu.sHtML


<!-- 参考信息 -->