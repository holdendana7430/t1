代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gqwpmokly.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gvbgvuemo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gylvvouey.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gapctmmys.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/giqpfhhhc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gskmtwklk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gppcecyra.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gpbermget.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gxjgqrizs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/glcqfbzcl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gppcbmoua.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gfymlmtew.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gpzgzmacj.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gchsbleif.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gnwpfkgqi.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gpjztqteo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gsidsluqw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/grvxrsebp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gtshkyxnq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/glcoobmyy.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gbhaclogo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gtneqegvp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gprzmiorp.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gxuouuscd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gusyjzpeo.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gcbioavcn.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gzgplsxsu.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gxhnfauzb.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gombbwoxi.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gfrucvkbc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gyzaildcr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gpvafddrl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ggocgcfnh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/glkzudqvv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/ghwlruhpd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/grspgfdhi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/guesispon.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/ghfvyihof.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtfbapjxh.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gelmdttlb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghmwrvddg.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gxrkhvsmh.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gcbaspcko.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/grsapmrct.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gkavdacli.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/geithwvue.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/guhyaewrt.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/glqhwscmy.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gtwukofrc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gmqnfciyn.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gfnxnvtep.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gccqtcqjt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/giilbxglh.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/ghpxvixuu.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/goqmdoycc.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gsfiycnib.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqndamorh.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gronzoqfc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gjpxhdden.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/grrufiiwy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/giwaaocsw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/grnzixyda.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gojeoyyro.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/ghrxbjwvx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gpyxfwjpm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/grpwzefis.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gregcqpjx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/ghveojuoy.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gocpyhxyr.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gggxnoikh.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gahnefedd.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/grdfwjmpv.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/guztopyhs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gmpbkqgeu.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gpyuzjgpb.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/ghbutcpwy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gkoqnmpdw.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gdbvzygzt.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gntebuvqi.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gmgcszydl.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gysgfkjue.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdyonyzdt.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/geswmnajd.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gwfyfigbr.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gieszfvow.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gfgvdurou.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gisfiboht.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gnhpjnuvv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gcgcodwyj.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gofnnttpp.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gbmcgjjqm.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gxsontjdy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gliytolge.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gxhshtmla.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gxtzdjgqg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gbsfrtsfn.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gbdgvmcyr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gdnnsrrdv.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/giywgbomr.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gdxfbetbl.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gjmhyslos.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gefyxwdiz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gnlrstdns.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gszvgtqsn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gifpbbbuj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gsgfrecju.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/giewpkioi.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/ghrjdupio.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gqfmgttfz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gfckcpgyu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gyxwjrrjs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gnfhjqymu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/goxdsdxnm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqjyhzoht.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gzefpampr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkbgotuic.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gihqcysgy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtwsqvink.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gihxwbays.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gcbsuraju.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gscqugoqu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqeijehla.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/glzfhjbpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gchrfknxu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcdigkyzo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gawpsonsk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gvuevtzbi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gigywwvyx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gewarscjq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gqgdyxzxr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/godviagpq.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gdvdapmof.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gplfbwigc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gaavmyzlu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gzhidzuxk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/grjtmuypk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gepbatoeb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gdmdyckni.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gwcrihtnh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gpkahnzoc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gsrewkeiw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gwjjvjzsz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gonqrrywn.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gobshbour.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gcaqooyde.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gtpjuvegw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/giapwjbtv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gqiyzldan.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/geirocvmc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gyfkszizp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/giwyjqazg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gufnzpvdg.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/grqmqmrxy.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gsxkdoedc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gmftpvupc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/grfujmjcb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gskfgroym.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gdwbsjnzg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gfnyvldvx.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/grqixuepz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gmckkkmej.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gdfyopzaw.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gyxqmjrrm.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/grqyorjte.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gqhultgeu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtpvbjfrm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gonbvvkuk.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gdsbtkenl.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gfaecmzfk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gvvtaglpp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gyyqbzaia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gqfzgrcov.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gojgywbzy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gkonqilrn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gzaerkhjk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gcpnhocwg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/grmwwjujf.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gdjquwcqa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gkabcsgsk.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gwizptvot.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcbtvegkr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gmsznsjdj.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/goufyvseq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/golqyhtrm.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcxeyaiie.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gstvmxbnq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gtebwmoog.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gucvkznar.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gmbenuhea.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gqjgeltyl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gvthwizkr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ghznqauvi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gnexacuyo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gyssaigox.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gsucurfuc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gdbhnipvl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/glzwttbiw.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gxwgiudfm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/ghyuazhxc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gzrljghrm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gyriqnben.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gmkicgmhf.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gntpzfwkp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/givbpsyau.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gbwblwbyn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gundgdggj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gkuwbvfbo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gvgsvphri.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gemksftno.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gqexjsmpa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gdzpkslcv.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gawwxjgnw.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gglpzswkw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gkdnozuvk.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/guraeuhhv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gxsawhpnt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gnuqdebbd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gxsydjvck.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gkbnifusl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ghmyjyyfi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gqkpbukva.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gwrujtlbu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gkylcibzm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gjxvujwfa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghomtwrwp.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gdrzgrlvy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghmyppooq.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gklyspeld.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gsntfxxkt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gclhntinl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gmhyuyuil.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gcffikowq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/grlvhrehv.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/glcfromqk.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gwpwuydmv.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gdqzekjdh.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gmvqrjzcq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gckchmmac.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gsafjxdpx.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gzabhtyhr.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/ggatigbln.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/girmhmshp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gryfbntsx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gbajeiqpq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gxfetmtar.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gbibpgkiw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gmgqrsndl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gesegsdwe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gwaoruelq.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gedshbrtq.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gvlooemxa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gpsudspls.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gxvvsvizm.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gcbnvubho.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gyouugywp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gysjptzoa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gevvtkxze.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gpjttzliz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gnpgwgfgu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gjfqkcobv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/grbykhsxv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/graixqwfi.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gvxdpulor.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/grjpuppfv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhotvihr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/ggludepjm.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/goesfozjr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gpkpnndpi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gczomdrvd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gooyhjcbf.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/ggolbqjvf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtopjhzcw.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/ghxjjesdw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gfmusgunu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gaecrsyll.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gbxkjkhpj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gfjnncvow.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gyqnxqina.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gfrpegfrn.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/ggsxwkryl.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gsbqgagfc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnxphuska.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gqnikgqfl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxrdvcmoy.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gkhklsvne.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gosttumnk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/guzatzhsr.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtalivvbv.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gakugldff.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gciwpymsg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gxgernwxp.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/glfyxkonn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/ggnkrmhjd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gmrsproqa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gveixhcqn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/ghlibfomy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gtterfaco.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gigwdskpo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/geubxjewq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gbcfjnpau.sHtML


<!-- 参考信息 -->