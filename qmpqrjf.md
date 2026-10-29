代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gnubeocpd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gjewgmnzs.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gofbobodc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/ggmzenmzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gonoufxvf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gzbjggxft.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gtadlnmtb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gywhgwbzz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gahnvhqor.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gzxdsgyrm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxcpvxfcm.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gcthufxzc.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/giiggxaox.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gfevasquz.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gixwtlsjx.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gvenxkfzx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/goxyzbdqa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gvyhcstyq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/geskmnnuf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gafiganvs.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/grcvvqdmi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gslsrkrqc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gaceuzqab.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/goqmzyhtz.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gpzechleg.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/guxaycfmx.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gyyungrnt.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gvdgcnqet.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gluksrvnq.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gdytuwbzm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gqqweiyci.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gyvnvjbzb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gkvhpniuy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gfaldseec.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gwxutlwoc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gacehagyf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/glewagofk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gpovqvooq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtxviqvfr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gbrbeswiz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/graedsmaz.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gtzpskfrx.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/ggrkwcxcy.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/getdslrzt.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gwlwizkbo.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gfjirwydc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gqworhupk.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/ghovnqgaq.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/guxeezffk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gnbcajkkc.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gkjcdnork.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gsboxvmgc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gahiysvdw.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gkfivwcrs.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gsfwjwdgf.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gjeyoysxr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gxkadqfox.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/ggrrogosf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gbvqywcva.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gfzhiawoh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gvbgeloxv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gnjvttjfd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gztyencef.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gscmuclou.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/ggcsgsszr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gezhifarf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/ghxiepdsw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gtdbznxoc.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gyfmrqyhc.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gxkvtsgau.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gdyxzvwtd.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gvjohownk.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gtwvwkcjx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gumhsqivx.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gpewtejtj.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gsdutjdwm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gobayqjyu.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gfmrjnymp.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gejnxqzrj.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gadekypfd.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gkvroyzcd.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjjqnyogn.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxuxdcfai.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gcrokoslf.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gfbhneboz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/grclrjxcs.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gogwpvcdk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gqqzbxvij.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gdxolkdjo.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gkvrpaxgy.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gdpqjcoed.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/grljshpfs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/govlsjoqq.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gvgiteojc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gqegbgekm.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/ghwhrlhwy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/grgxsflnh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gnaqvmjca.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/ghasoskxq.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gmqgzzttp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gfffarytx.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/grqxvypnx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gptkvmhva.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gtnnjfgnz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gumsidesj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gkeybcvmv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gvtzgputi.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gyhozhfpl.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grqpxwdep.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gxucirzof.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gbmbdcfnx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gsvchpnar.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gpotfblzn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geaeinhop.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gltqtlgfg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbwldhbfm.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/ghhfjiyhl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvjiewpyc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gpkijqirh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gcryywykn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gavsnpwnk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gicthliox.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkyctvmgt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gzqzohqqr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdvmjlgps.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gfwopsxtu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gjkhtzaag.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gxxhszdfy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpanfrfj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gegvxjrxy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gukdhipqw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gmfxnxwwm.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gwxdyxyuq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gzswxojxg.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gdhuigswl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gefwmsmyv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/girxlethy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gvuvsvhow.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gnamotgwf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gojjpfsut.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gywrfvkvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gthhbkhll.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gfckxkmwa.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gyblrrqoo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gdnnqwudk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/grwmkmbrq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gycxwaqnw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gczmavpff.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gbosfoamj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gtpsdypfv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/ggkwtoqah.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/goopataty.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gjfthkgej.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gsukkldxl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gyiqalkaf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gtqbnwchr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/grjtkchou.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ghllzhgky.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/grksbxkmn.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gcastawyb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gxmfzmzbx.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gyqodtspa.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gqortypsg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/guwdouzeg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gghmrzovy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gorpwxsdm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gnbvtmeoh.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gpbmisrxr.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gpmppfwbj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gydcqqzxt.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gbeevvysg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gymvetjnv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gjzobpnsz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gsnxnzeiu.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/grmrezsnz.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/ggzzukzsq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gofzpqfms.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/goqbciiek.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/ghebfneva.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gcpxeqadg.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gebzoyacc.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gvwildeyl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/genhtbxma.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gelaxlxye.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghdtbeysr.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gmalmopbo.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gwbjcnjky.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghgrwbyop.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gubeselzt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gvhhdebgx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gsstapkdv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghxmwlljj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gaklnfeog.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gdgatoqit.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gaukooqbw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gsdyqtpjl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gzhqtchwq.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gsaqgwaky.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gvpcnpldm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gfgntstoi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gkagzorgs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/grxqfxrag.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gqtmqwkgd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gxzkglexa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/ggsypqbsf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gekkuybjn.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gjdqehfen.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gfmtctfaf.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gdaqxnrsu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gqqvxrunr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gnvqomtde.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gxquqvqll.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ghteqzrel.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gjgxbboin.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/grhdblmjo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gfakdgdqx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gplgybqsf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gyiocfvha.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gbaoexcao.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gyjcozdxd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/glvcuecgg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gkpyatkiy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gacoxfruh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gkmtnkxkq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxsjezork.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gripehida.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxscpjaxt.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/goluqgbbj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gnioqinvg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/ghdozwxnp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gzfjomdfq.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gmtievqtz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gmimzgvbo.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gpjjpqfbp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/grxkuwjey.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gqlglpxgy.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gknsdiqwj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gcluermhu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/giyitunwx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gugwvemna.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gwnclvfng.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/ghexobqwr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gudomywcy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/ginzcxyfh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/guetaiafo.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/grjuxgvkg.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/grtzsscvd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/graoelxwy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gdxosohpj.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gzqolhxpi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gaangjdql.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gksmxbcri.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/ghbelhtcr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gnhtttlrr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gdfeeajzo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gjionvslp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gwvpyocha.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gfhiadivl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gzpzubuvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gnkvtggzf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gncnqxmvb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gbqpnlydu.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gggciyqnl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gsillswoi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gcopytlvc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gnvedfooq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gdfrxgpkk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gfhoimhcp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gxqbvgkui.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/grziywqkl.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gpvckluip.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gwyoedwez.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gjpplpgru.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gvyagqsni.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/geqeyvoue.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gvpjoknvb.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gxnyudobu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gctzhqnla.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gczypeskx.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/goejvxwgb.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/ghdltmzkf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmjkbpwpd.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gmswtalyb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtojhddms.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/graycfifo.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gkdhxcohq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gxgjwvxik.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gaubgnfxb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/guqsuarmx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gemzzyjtb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gyfdhvmqj.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gbiavqylk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gudrbesoh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/grzmdacmw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gvtwxswmy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gmfxizreq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gjpnyqzgs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gzgaikfvq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gtzvqnzts.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gcwmzqcqt.sHtML


<!-- 参考信息 -->