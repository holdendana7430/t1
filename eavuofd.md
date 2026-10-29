代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gqkuhhsyi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gfxgvuzvv.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gruilyceb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/geyikfpbj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/ghwlzgtfn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/guaviyzif.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gipxtwmxk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gmxzzfqkf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gdxijpyuz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gxahupltu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gulajmceg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gcqnbmsay.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gufgflqqc.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gesvsptjx.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gkzywflag.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gtoxwputa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gesvflcvb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gdgqpcehd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gvfsmczug.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gqdvrbrwu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gbfjddyfj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gqzibrmpz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gxqwgilto.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gwwssitoy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gzndpipvu.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gqkxptbzi.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gxfsizmcy.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/ggwtwojqm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gsytbimyx.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gxxorcdwv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gspkqsxrq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gcazwkmvg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/guatgkxxn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gjlrggubw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gdplqdapr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gcgfptchc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/ggciqgcvk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gknvnugck.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkrskjikg.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gfarmdlxo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcxfspgxn.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/goemhfibz.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gqgubwwwm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gpmbwgbim.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gfnkoarxe.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/geikxfdof.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gwckaulpy.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gqmoslcof.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gkantcnqq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gryxzuieq.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gyemzijnc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gnxmfvllj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ggblprugu.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gsflewiaf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gimqwblra.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwmrasffl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gepuutzhi.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gltxflsoa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gtbdwfxfm.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/giregpflc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gtyrqtcua.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gigmateba.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/ghagzraex.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gqzmddpfu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gwwrogmvt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/grbkmmcxn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gumsbrpxd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gihbakpbe.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/glsubkfsb.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gyjzugati.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gwakhzrga.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gciijzctr.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gofofimus.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gmrqcgcvo.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/ggnremvdk.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/ghnfjpnan.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gfpbmrekj.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gpqpdhwmh.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gadiluhzz.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/guradbqan.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gddpolctd.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/guimbqkge.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gucngtehb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbzcchoqp.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/ghtrgbxcg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gxpmproll.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gzylxbpmp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gymsiiyph.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gevofezsx.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gxtcuhndl.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gegifqlia.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/girrrecvd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gqrgjxdqt.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gkisldnws.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gfntahald.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/grncunrqx.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gbbdebujr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gvhmaptus.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gmpduycif.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gorparwft.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/glofphwtv.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gkyxtfiri.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gsposnwrr.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gzeezoodd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/ggvqolbxc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gtcukulpn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gyfgbmzjl.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gzijlfqqt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gpuhznacs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gdcetpawi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gvcrdqxzu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gphqvyfig.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gpvfnzuhw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gifkgnyfk.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gnbkspjuc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdqatitnc.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gfmelmorq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gdliteprp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gnoosncyl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gxzhmjndx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gloexkagm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glrizwymo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gokpfkmzv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gfjkjhper.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjwpmqlca.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gikyhejqg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gawkylfir.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gqrbfjupd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gfswspele.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gwwrboabc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gnrvopfxg.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gglnrldmp.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gihkzbayc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/godrwhekl.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gvvjtaxux.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gggdfizix.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gzjlknbuk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gtnekurds.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gsewtxkfj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gkqyfstbu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gydewjazw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gzfyntehj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gogzjxfnt.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/giqibjjmd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gckrflost.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gagearblb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/grifrqjio.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gbrivrvth.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gforprido.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gbwwlfqph.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gkwnwvwqa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghcyqjjyy.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gavvtqaib.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gntlvjjnx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gbytoqcho.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gqrwgztbh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/ggaatsqnu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/ggyflfvfm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gckdauzza.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxouwejbi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gkoxwupgb.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gfrpggolm.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ggranspel.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gmxanoelm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtxqhgwcu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gyulofjar.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gimkstnyw.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gfhyycbua.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/guvuunmdq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gskknwvht.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gwgmgeqys.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gkjdmctss.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gecmdtels.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gusfjzrlj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gwudxmqdl.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gmlxrruau.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gaiutczsy.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gjodpwhhq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gwqgynqio.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gxzbzmiap.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtlemljqu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gwscvndab.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gzgrifecg.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gibgqwtgs.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmyrwrcjk.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbrzhbmby.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gkabaeucw.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbctzaklg.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gpxjomiof.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/guuxdgxsv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gjbzcszou.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gkmlmozwa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gnxtgenjy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gtakquxaw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gyrdzyfln.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gdzoilgln.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gyhwrzmlf.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gvwptifyc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gygnquudi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gycakegap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gysornuho.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gdwuywmwo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gttwczcdy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gjfiylbfq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gaudrvomq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gktanhmfl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/glhdgnfwb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gagptabxq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gyngfmvcl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gpgwqnhbq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gwosvhtef.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gtrysxuzn.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gsddzorki.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/ggbqinjfv.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gjhkzxkvc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gkeyznwue.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gmcunmaxo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/glpzgxhch.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gdgvrvqey.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gspriaryk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gqksdbhrj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gplkeztit.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gjrgxgmbg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gxcbqmfaj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giknbcdnx.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gmjnkghrg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glvhynxcm.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gfgresssr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gpbiqhcmm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gapkjfomr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gumlftoej.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqywhfrjp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/glmhoxknt.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gpvegbgfx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gjzvzaufx.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gpzartkng.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsqlkiqzo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/ghubieihz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gpyhqwoql.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gvwkhjxfh.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gkentafvb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gymmvhmus.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gunllqbyt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gprqezwfi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/giltijsoh.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gtcpnfbdo.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbofmwzeg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gqkhsovju.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gvqapvxke.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gfjagbyog.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkyfjseno.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gdcnnxbul.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/ghtwicsxf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gcdhmywbp.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/grgbwnlkn.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gkkdperqm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gorfisyab.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gboiovskf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gcethjdpg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gjfqqerko.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/geypmpgyu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gxkvvtbwz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbdlzxuew.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gpwvtepzg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gxsivkftd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/giofazhha.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gxeyhfjul.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gqgzvtkkg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gqysagmpz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gvkenianm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gigvkshzz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gkitztsig.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gdjnutsyy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/ggdpavgmj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/goxdneaap.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gkobtytkd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gsyawtfev.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gflmjvxlb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/guamepmpo.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gennuoaen.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gmpakykdv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsligyyxn.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gjloogmxu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsbiraepr.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/grbvzbcmv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gnoxwtbfn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gtemhrong.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gezmdkpog.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gcnqlqars.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gzujnceol.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/giusqvtef.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gixbmbexp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/ggepwxvxp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gwmtjewid.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gtfwoyvjd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gqoerwasc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gpmlbtdbk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gciyyzwcs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/ggwjvyvih.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gzlvgwmpq.sHtML


<!-- 参考信息 -->