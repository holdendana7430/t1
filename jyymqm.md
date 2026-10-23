代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3crmdngvo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kzcurlms.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xaitdisv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hkxxuamc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3drqklcax.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nmgvogft.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nvaftfii.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fbugleru.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ruhhvraa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fgkjswjq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hyrhtrah.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pacdqoyd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3dhxdjcrr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gxxjfght.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3uwyicnoe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3idihvmwu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtwhzjbd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3carinhzj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ljweghbf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ahnwweaj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yphxtmuo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cjjgfbcu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3btlxcpqy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sdamybpl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3erykstjf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3xjumtotb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tvyshkqn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ltvvfcwm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tnzgzqao.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tszravng.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wypmyjzc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ouwvluuo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3btjokypd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mddajmxu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hrcrhrqx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wargqfhn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tbmqbhlm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3syersono.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3djbuzbwo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zppciuwt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wnuiabbq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jwbdwtlc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3eshhkofh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3epvlphvw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ekduviue.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wxpwyxso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcxjpxoy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jeqpzzue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akfjwdhz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vspqkavk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3khigjwpa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3flgovhhs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mggdbise.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukrlmaic.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3huzxxbpz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mijzwnnt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3fwnlbccp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3movolnra.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nvipvetd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uugumflr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vmpublbr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3szrsfbqx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cfyzsqkq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lguafpqn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ndrlgupr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gdzmwcly.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yektuoxu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qpsbhqka.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hktrwueb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mvwpaqaf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hewxcoyw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dyukmdmz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vmyswhsp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xfankbfi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dewzjtco.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3rpcagbul.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lufbxkcs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jwdxejjx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jxqmeixs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gtqukevz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uiaffvuz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3inytxcfm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bmluffds.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3cplauvks.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3krroobuc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xvgedpku.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zamltcsm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pcbxupin.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gforybxn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ankvfmaw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glpkxkoa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iazmsplf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3jfdgbfkl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tugrbzkf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ewgyhwog.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xxewirnd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ufkzqtcy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3attvyerp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3popdgmvk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ievjittw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fyeccgqb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3uctvdgor.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3belaosqi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uavsruih.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ukijajtl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mbpkapmd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vlzztzof.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xtockhal.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xuduvhte.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rwvcyakv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xjtradaj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3aapektuu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zkyzdtfu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3smzhxcvt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wjhaazgm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vysarkgm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nlyjvebe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3msbnzbzm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3uxtxvkht.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mybsmdfd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qothznth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcexttpw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3alxcjwft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxxdmnxb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mmuplbkm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekpnfqwr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pnddwsgu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bwtrhkjj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dgcsrufl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vkgzdgwh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3igrlcuzx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ooyfiazl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hadodbkf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bfobgqjm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mznxcgtc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3byxofdju.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqxfeby.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ieketxcp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3plaxitjo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3msontoly.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3braxizps.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hofagbii.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3paoxolvg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xiqtlimy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3koptunrj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qgyjsurp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ypoipymp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3prvdbxzv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qjvkhyum.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3guodoqkp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mxdtpasj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3myfuihro.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qssnmudm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xijihrzz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xypfbxki.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3psgxmeim.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bnualceq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3okzdssji.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxuafnsr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3skrvuuga.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dyntbaxe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ntsubkli.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jtamzjpb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tihczwsb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvrjhgoh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wnrepvkt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lcsvbumg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3spivzudd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3eavagmja.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uhymtycd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yrroyxfb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yukwidyo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hxxilvuq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3limgnoha.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3oizingmh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fzkysvgl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3clxhumez.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3egihrsdn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qmrkhzhd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vietdmmz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3vkmadqca.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jmijfols.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mdbpjsex.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fdejiqpe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3tozkrhxd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3uxswdvbe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3delnuill.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lodbqjrb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3imlfyqgx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xnyvfjve.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftdlpokl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tmjoavhl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jtvsktur.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wxucqlmr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mimubris.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fwhuycbl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3psnxqsfs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ockutjda.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lsafjkyp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yheyyljg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ulsfpzec.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uclfrkgx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pblqtnhq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ssfjcfcm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rdcxakhq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vqfkbszy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3paabaxba.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgifnyab.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fktbyesl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fnetrjkr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zjiklnty.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bwmjlxkl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lctlagua.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wukhcakh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ywdsxodv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ejqcnzqe.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pkvpqcnw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yrxslcox.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vtcjmclc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xszhudxm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xqnvarhu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xsopaoyx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xsuqxsaz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dwndznpb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vxlavgzf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xuphftxy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dkteogwi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rcwgyevd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gndoqgxo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqlhdsw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rigeegpj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3omkotmhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezrwquhy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ylkrappx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdgiqjpx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xxhborir.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eqrjpikz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3wirhfzfh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xsgjknuo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fvcmsrli.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mbmdlhhb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ffyxfuht.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bmphhqhy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3gfzaqval.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kvasdpgh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fpvteupb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3yhipxmpe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3njxlsobh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oeihfprj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3hjmkmdwv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3azxcsqek.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nsqkfpuj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dwufrfvl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hiymmgro.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ulrodsvy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ncfvwjrz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3khnlddgk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jatggsdf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yijdfayz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jaujottc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3uvvfonkd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wpjdlchh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jqokrkfp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3dqjyblfi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3oyarpfwl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcqngony.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3quxunyua.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jwdbmjce.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hpkddkri.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dzuojcpv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tubggwcm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ncwpysjd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3edyaoqoo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vemsikdq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qcdfraby.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eqofnrqe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3iuoywfne.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zbihjixa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tcwsrlcs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mcakbmud.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pylzqwuz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fuokqfxi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vxrbscyn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bpmwuivi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pepfsmos.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ushxxpwz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lwufgmte.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wiifezsz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ysdzmuin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anajuhri.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ahywmqxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kluzanlp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jzhtyybd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3msjcgitx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wsfonyet.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zmpqjcrc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dkjmcvam.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ugewblnb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jelxprvt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3kdpfddnn.html


<!-- 参考信息 -->