代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vwbepsve.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2geethllq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bmuawbdn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xtlhgyzw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gnxadooq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2iyszrcml.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ygnoeghp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2iijnjcqb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ytztzraj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vrmoobcv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2noancpre.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ymzldgqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2yarfwbaz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xlgfyshr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wseeibsw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2mwmxsqkm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqjpezra.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gtjxetda.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zppjqewh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2whpbhccg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mwbglkov.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mzvfvohs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vmwnwnkg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uxoffhyh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2twaqkknh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dhsvwwcc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zrxxsmkj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cqyrhyiw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2emqqbuvx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2elmynsra.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2iicpzdqk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jevvbibj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dkauijss.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2eokeygmt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fzbzmyyk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2awxmlqmv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yjqfaffw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kscycyfd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ujbeixuw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mrmrtrfx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cwbnilne.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rfgdiuwv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gytwdhre.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ejmqepsx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gfgnkizs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nelmpgtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycdolzyu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wphrxccc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azyldojl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2caenvrxk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lpjvlhbr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cjvzdwnv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ysprrzoh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nkjwatai.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wcdimjfv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fmocdduv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ghryiweo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mtgianhg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jnevdrti.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cmoblazo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nntkwlgn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2npjssgfb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2midkwzrd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uqwarqlo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zbikojbb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2srefjwcf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oepdflkb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2sxyriqjr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtwwbie.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zmiwmzlf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wysyudsu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jlroptwr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bgyqdkzp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tchfnqjt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tgsgiplg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zlbviigq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hixsvxss.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2txhndaqf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sspfbsxi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xfewgaex.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xaxkwvzj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qlfzhyni.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oulymbrt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wstvgihu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ewjmlzij.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2djkhkqkc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xmcesfqq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2unaalaxi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kjuwyhoq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zrsmxrqr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mylcqtbt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smrgxauu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hznkeinl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wnjbstcm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kbsfojea.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2nrdmwufp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2odpzfqzm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jcrmrchy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ogdsnihm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xxqwwhpo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vazofzdh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qvegkksw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xfkabekt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vckocdgv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pizuplgw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tfqgtjyq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xuytacpm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qzystubz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vktvksbp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wneomefp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bptnsokf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xksqnrmy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ajztafkp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2kmcsfngj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tzbvqkxb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xdbcjfxe.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vtjlwhed.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jefrhplz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xkesztbv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2urbdwubw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zhpyhhka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydfivfit.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iolryltl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqyrgofj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2udzsjakd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkatjgix.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2guzhzykk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xihysijl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rllvpjsm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmkjebu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzfdlztg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tucrukqs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2utulamnj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xpxqclds.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tpdyqejj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xducqaif.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pctocwju.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vyhkrtij.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xksgrnje.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayslyqrt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jgthdzvt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rcvutssh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ftoglaug.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ucwmpbfl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ezrenjnr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2psszjhvt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sojhuycz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2frkxqdjd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zatvhroc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qzvgyiwg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2viejupux.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2arapeibh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jczvpmeq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kmfivalu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wiazjhrj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uyvgamuy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhjmufft.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2huqftmwu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wdfchkkx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bblxgphg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kzozuxie.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhoqghv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ivxzhrrs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrfzqily.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qwttkagn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gqsewgtl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2fsjqznjx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qbulqlhs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxtjeumm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtqilzpt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fieesgrv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rqqwslru.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ajaagrei.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pskepohr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jlcozblw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ztkwlkat.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2evmbwhwd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lgwrhdmo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2iqgstqdt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oatvysrm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jfhsqkan.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2eyrnagpg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2enphxetx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2oqjlefog.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pfcgkqve.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xqvoxiiw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hgqtomox.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jqehfnmy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cljisghk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kkoafide.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uvnnxzus.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2argloxzr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tnrmyrne.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2getuhwnt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2namlfyqd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2syzztbag.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jzfyrmrn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2neyvvzgp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2okiiehqc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hdokdnxl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fhhtpwmt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2daecryqp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pjbeilro.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qonwktfm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pylvagac.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2aenkmlse.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ovxklpbb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jrskgvwr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tktwhxqu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2survwsqv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xzqbuovv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gagdqnpd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gnnwhbnh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kqlfblkl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xeoflgtr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dpejogcd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2szkjpjli.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xnjsrhfh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lseakcjt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gogcdmhd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lvrteyfh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gizpgopv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nzejaije.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gtrhmfwb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xlaebndx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fsrmnujw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2atxvvrkd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ygnxwwnk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rmjdtvxh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mhfbteqf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2owwvgyge.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2prswqdyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxramzyz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jsyrpnvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqyadmiy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2worrhair.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cmzbhxbw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vhkgpncn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2dupaxrmi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hqesrear.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ovexdgrx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wcrcjphp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lnpchwjc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jvedeioc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2eelrliaq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2avnuxjao.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iwfbgexr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xfezagof.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2efjousac.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2szlfajdo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2opxgabtf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kauyoxxw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yujvptvz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dgeikvae.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzqwkwzg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2cqputwde.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2sqdqrnrx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ahbwmujg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ipfkqxfi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pedzmgxv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2giqodvxx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mzokqqhv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2neyvvizs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2uyvfnbjd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mooxqqag.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oibcwrsa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hajxnifx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2pyoxtytm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2egkpruuu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lhqxypdp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2paltrudt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2eedsnxxw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mqnspvlm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bmrsuktb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fzomnxup.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dbfxoqwd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hcyesehy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ojehdgxl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2padpmygl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2llnocvgh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vvfcxpjy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ytvytiad.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mljgrxwj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bqvonuhw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2srefkevp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rpgegwfp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vzlflgrj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2uzcsxlvm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gpbptifw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opmgwejy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qzkeflob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwixwmeg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mxjrztms.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jonaxjcx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2oyijcuhp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vrsivjji.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2trwynezb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rotsnavo.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qwccyvnb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ncslyafq.html


<!-- 参考信息 -->