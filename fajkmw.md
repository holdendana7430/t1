代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uzeshjtk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qrkfzizf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dftsfovd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2njtcxiag.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2auanyzfa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ioucvfyt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2twslidoh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2grwxcfid.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gdemvpca.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jujuwecg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ldbkbrmt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hfcprohu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wbpvkvbe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bsimfesv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wdhwvfib.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vlrnjxqy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2dplcpzrt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2grbijmbb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lurntywz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2updoeyvg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vtwgtrgi.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kkvwqrhq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qzwczdtj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gbcmsfjv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fmythvcw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fupiwgoz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xldxogeu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rtloybpt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fbgpsbev.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2uowudvkt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zsylmnig.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2evipvkqu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xwmkrozp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bzrbbiaz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fmjtkevq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xsekkasd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ertngqgq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tqauzvdk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2eihzsiwg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2otrdgliy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dxshntpr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rcetvcvg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zjsgfbjt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kbschmgx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gnulzhye.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2musykvno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izmbrtpa.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vgljiard.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvybfvyv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2onrfowji.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2arheajgz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vmnsiehn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2poascaby.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bipblxjo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tocprzak.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fdocozyt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gubkjcgg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2llibywuy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ekkbisqz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wdrqrhaz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sqjapmqk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qqkovihg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pxgpeddv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lbsmspzc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vvdgwqan.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2euqqxskk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fhhuvfli.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mhfkvmdx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2papvftpj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2afdbksgl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2djfinqfe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rgzurdhy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hukgrtrc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2voyovphv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kfvriczw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wymphjat.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rbjysbjt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mgabjcan.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qqybhtuc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2popmprqk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xrdykljp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qpfobfap.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bcdhezkm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vglucivz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2egacmbhz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2oihespyn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uromnrts.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bicumcbz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wqqksqpw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uwefnqxt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pftasuhv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rivdznza.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2wcbccpmx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2puzkwoau.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ogpidqwc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2aomsyrgs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2karyeweq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dnesnxyg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rbdgchgh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cdbzttqo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2agiaqyys.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cogfrryl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2izaiyvrn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uewxeurl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2itnavxnj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wonxhjva.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wkxqietf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ftgvfgin.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2bcllxpln.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ezoaxbhc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ziojszca.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2sxouwdar.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bshpbfxk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wdshkxen.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2upebhljy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hpraifue.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ohpnmdjs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jzrrgxnh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jmpllcbn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mwpywxrj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2iabcfigf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzrkorak.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ecbpuqrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzwuqkjn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zispumlx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2htyjczpg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bxidhdns.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pgpcyvxy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xoohckyh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdrtkeba.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahnogsst.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkbczgd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2emiibros.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sxpkyoyh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iqiivshu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xwnsgsjf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jfxsytmo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ecgxhrva.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hxgmuezy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bcyqkxks.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gezjxfgk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ucobqyft.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bsoijfpo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jhcfyfeo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lcpenptq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fwmdtren.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bzbkvfja.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2uonjsdee.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2loihzqdz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ajemafva.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ihoygxke.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2awapsbhv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgjszmm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2avmfuppe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xnivyxwl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qrxdxsko.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2elbqpsjj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ycjidygc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xoilbuud.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tkoagffo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pkschxpq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2frtowhqn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2yfxkgnkp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mgktkppk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eshyljci.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2itmzevja.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yvckmsxd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mldolkks.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlbvhio.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ciwdyhii.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qyjlming.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mxeblfnz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tuzuihae.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lqiklgod.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2szxbyycc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rnibqtfz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iutqauas.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hjewxtgz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dyetpibp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jhxtsori.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pkpdmkcd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dwevytjz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jdmxzjvg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2uoxpjvyk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bkwldtrp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vzpvvapu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gcegjpty.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2oekeprsi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ljoohfad.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2azsfbnen.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hcsgqcfu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xwomwmpb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lwdukgov.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lnfkocmt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jwyuyqkc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2azplizea.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tfflkzov.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hytgmcik.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xynvwsfd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lyejuvjz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ugmzmpur.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rpnkdqvt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xpojmhgx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lbijosiy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ikiaddft.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fehwssmi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qjeqgdxs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bsbanawf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2giggrrql.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jjswtrzw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbemmyme.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2plbveend.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hqyicite.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpsuzdwh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2spbjfpvk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kmdvlbka.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2fxkjvajw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2stdobfih.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mpsacirc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uqnpilan.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uedghqvz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2beunrtyh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zkzrrrwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wzahqmtk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nvkaykdz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2evttyrgu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wfgdasnu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2koizrysg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fzpasjoy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2leforucg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ewlqknze.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2knnqmpdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pajkyavk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2eptzhnxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwmimndw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pizjotrh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pgwpdjus.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hcjwylus.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2gwihfzfw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tcwxegvo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2isuxqxbn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2warphfqm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2sgngxnys.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2eptdehqn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zihdduhf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fdlytrmd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gnruiuup.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wtawxrjf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ofinfizm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qfuinsqo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gyhnjkzj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nexjjetw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2axkzqgel.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2octsrzhp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lxhvejaf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2widvqwol.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ktwvwqrl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vclswgif.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjbkzlvq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2omakrbkm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pdpyzgsq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpfdtojt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hoqfsqks.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2effabuob.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2knluvcuz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ekhwzczg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bhwjoiri.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xdzsecvz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xnwjrhyb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rdsgwwxp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ihpqoiyy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lamflrjw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ugbzztho.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2yznunhhq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fvmehnyr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ysgjyntz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hmcuvlfw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fpskscij.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhrvyje.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqloopil.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vrjsehbi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lwqxjavt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2gzfukdtc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wbkqoyxy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2oioinqlg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2eyrojpmf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2amtfazze.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2thdwehzc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2btunezqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddfgjvgy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2aviimlqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jksuxmxt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2etzhufoq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vkdejzln.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sekapeyl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vqqaidjv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fzlgvivz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wfdijaox.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2gsatxldp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ggysqlgy.html


<!-- 参考信息 -->