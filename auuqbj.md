代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sxervolk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dnpymtiw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hcgyrich.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eoilenjf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fccouceq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xisocrwq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3vizlfldv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wfsgdbhx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3deodlrnm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uymmabkp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3hpoervid.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xpzzujre.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hyoiknqt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jirjendn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dguizdjr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mvmqxarp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hrvlxudw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zgeaoodg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ahalwsbk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3opzwwxpt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sxiiemqb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jjcmjgxo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3niianadc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gmehkglt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tfuajwlm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gsifbplf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ubzrhvdw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mdibrxdn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gmvsfdkx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rnegspgl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mylslfbd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jxctmgvj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kutohwlt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cfoklsvg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bbpzskpk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zttffrtw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3udiwlazp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ywuvhwoi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3coahadkc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3tdevgdut.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3utnwvtqa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eehuzmcs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pgdnklgm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3unevmney.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oktelsrw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3upknytbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgseekan.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kzpbnqph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ribpziup.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3waitoyhn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zpkumzqv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bmppwgig.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vpweiqvp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uitlbsll.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3skfdgktl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kdqdyxtj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3oqdbwnys.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hekjeptz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3evroubab.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zfowhkaz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3axiooecp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dffffvfm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3txhkwvin.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lujwythc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uycsujvo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xkmacekc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cndfbbey.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3czjjvais.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sdmqabzu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wvfhclxc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nlqextjl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ujrdgrva.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jwuypfho.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3oadlccje.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3yogqdipg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uhdxvsyt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jyafvjzn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uvyerima.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3krunylql.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oizfocoj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3weltsaun.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hwssmhaz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lkymiupm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hhcfyvpc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3fgpfqrxr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vxikpooj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohjfqhtl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnjlndt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yclfyojy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yupzeakb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3koaidtbo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wdfswxkt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3erjmfcwt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ufxqxdid.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pyheabhd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ytymkeyg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3dgiptqhc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tfutaqhy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zgcugwbx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vrucnpwz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gxgchzpo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jxzgptog.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hqmkxfxx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kgcfksjq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3iuwncsnr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3aghknajm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3krmtrhht.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3occznxia.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3peuokina.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hofcshbi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3sijflznn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gmjjlnwg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3sgnusqfq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oghbhvcc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rkzhswts.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gsmdrqrb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3paldplhv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3sdpcosie.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ixjqyteg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3veswebdb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3akwrhsii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vanzpybp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cexxffpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoryxtyf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ddttsuyy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iuucfyly.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ijswvzcd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yszyvpnh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bwatigwp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpaasrfw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pvxdesep.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gxsrkcdf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kzwqnhfi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kugawxbb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3avhmfggy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vvcrpxbc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qyunwjyx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ilytkvmx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3maetjtsv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3keeyvrew.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fanmkrtj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3edqezkjf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fyijrenj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3prjxmqbd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3amykfpjr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fvmfrjxj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gfngklml.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aielkmne.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kfxwhlqz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xooinumw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3datazjlh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ttahbobv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gbymsgbu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nbnaazyo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ewdxfvtn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ztznhqki.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3omfmpldp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lcqjfnif.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkdgbiue.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cdopzuqy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kkncdqcf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mvbhbepd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3htiywuuf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3irdbksph.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlsifhdk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wliweogh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jzdgamff.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yvezgfrh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tbbjafkn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xliyirat.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lxmiagoe.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kgbalmoi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rcmrxgnr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mgeawval.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ozuihpxo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fevhvvvj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3eibbkdny.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3czvpnytz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lbgzmhbc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3duqrqnwv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ilxdpqzg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qurlawxc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3eapmulyk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3eabdfvkz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xmdcwtgb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tsbvybsn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ywhyoduh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rciyjjmm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pnpzefpy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lkndxtng.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3prfxtrcf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3juzzrkwh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vpopskxw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3arfmqloo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3skxmcvyv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aihmwxva.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kbxeiova.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nukrsdmw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kwxrgnwg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mlkxvcue.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bawkvjaz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jhvzcaxg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3sjpndjen.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ibaqqclq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ghihccqb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3aiozvyut.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3scsefkte.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3flzsxnop.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tyxdxhse.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xbokyfxh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xxslsdvi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wuupblcu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ubfqujdx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sijqjeic.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kctbcplc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zeulreqb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3oumtrjss.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vjvctjwd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wukklmba.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hlgfpouz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qmhxlomz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hixjkqxm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdqgdety.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wdfjppuc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3whvsbtbd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mhavgmtd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wtfldlfi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3sgvzklrc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kpdbrrfh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3jpmyeost.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lyfxarwt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wzjbjlqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsoyuoos.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3aygmpeva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjqlogqd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ceychian.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hahovwgc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mlknctur.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hzqfziga.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gavlzayr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wttwjosh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tlthhukr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jrnrzudm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ulqwvitq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ihaattit.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cpcthqzl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3fbftvtnc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fswjrtke.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hvpakbjg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3odaadbnm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yjaqyhga.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3szgssvck.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3htxyvxrw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3doxdldug.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgezeyzz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3radiiczj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3krapbfda.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mltpywte.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jbrrqolz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3awlebopz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ozzcpprw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rghhndpe.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yfrntrpv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vdgoscuv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vuyfwxdy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvqccbdf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3agonevxh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3poxkudtl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qsqqkhbj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3efbximjg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3abpuhodt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rcdrdwxe.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3himrpwzs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3dziqqplw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kjghzezx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xvbpyqww.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3agwiqzla.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3huepwprv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uttuzibj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wzhmqtbm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3pebhtorj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qlhbsvus.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vhmcxmex.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rcanbpho.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3occscxlx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fquloyoy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3hcbpngvf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ymdxurfj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bxowoukk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrrjwrpq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gmailtia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwcphxek.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3anigqomd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hvjrhqnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3itcxccdw.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qozecbct.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zqgkxazs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zbasbitp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tqnroxnx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ftekgder.html


<!-- 参考信息 -->