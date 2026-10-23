代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3drvyltkq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xdaicwik.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ixfjrbao.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dfusoozu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cjkppirg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vlftbzbm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3czqnpocx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gjcafixu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jhyugfut.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3duqxfagh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zvoxrcck.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fkvbhgnv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3vtpcyuqg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3mqhmzied.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kiagvuvw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3merorhjs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xnyrvlfu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hbjfjgmr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ulnwdiex.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3hlhzizhr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3wodmmszg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3piuarrnq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3budhjlbp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rripqcpb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tzohmsuc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ihyasihx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qonukjwc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sywgmloy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pfstvjvf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ewzopdxy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3szorjwek.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ufharice.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qfbxxsck.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zlyahdnb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vqphdffy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fgthrxlb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eebltznu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3espggzsw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mkwzlmeg.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vkxzdgvy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3sswmrujs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fqjwabzs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nskqrlin.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mqrbvjfk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3msgtrguy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oavqqsbd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gttcmxvs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3exvlbhuh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jzlmlqhc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3derprsam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqiridyz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mbwicpau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apbdfscu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zhrdlprw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ixkucrtm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xfixwmqu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gqnoyjrz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhbugwnj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cccksgcc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3divoulxi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zsrkrfzb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qffpitgo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3frmisnrt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3glcgewie.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3utcjqbiv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lwjxnqkd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lbtzyzfx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bgdikhed.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjztgcd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gnublbgj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3icykduys.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3atnqhzco.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eoujcwrb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3iwgppmev.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wclgckfs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pyycdudb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ltksmari.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bojrwcuu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zrbuxoed.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3bufehumr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ypodbmfy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jrqzoxct.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zawryzpi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pdegubwg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3luhitash.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3aypyvbtc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vkefeiyp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3namanece.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3eurskonl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3igpjerkh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3isxqgdzb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3savxwzgx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuubkpsv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3psckabgd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3djmibkvi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebbivlyv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvisqsqe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3komgalpj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cyzascll.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mnrrpjlr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ddnzdhat.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ggijhrep.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jkkicsqi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ijrqzadt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3neyouphv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vlxjmiof.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3swollref.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pbffvwik.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3liruhlld.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tnaxjeee.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dlvqsmvp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zhnjtuhy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fysublco.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cqrqpmlf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ikivhgiw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3isspmuch.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uknrjnyq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yetnlloz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hprtndjs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ruczolqw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wvtcahwj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ouvdlkdd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3duigvmen.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hiuuesnk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3slefzgfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lweybgdu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3sfsnvvuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fltvlnmi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hcwagfgc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtnucpnl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wqrhrwvo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iensedsz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gzmwzkfl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3msrawxny.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ntpegaez.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lzhwsxvr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zoswjsjc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3plcqprkj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ythuyszk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jnaziwjy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3plgkygdf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ighwtirz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqbomlq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ibbcrffd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ndgxrxxx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rgibazhu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3srxxexob.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cprpfmsl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3urscjqtr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hesstbip.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fygoocpb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3eesquzcv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vlzjzzuy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zdbeztvh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3semioiue.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3oaxjqzpw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bygdoryu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwnjtgnh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jggzpcga.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ocmaefsz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pnfgjian.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qlrtrvqe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owqeqamh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rwoleyzr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3runeeydv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wjgackog.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tmnswxpd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkmuinat.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ygavutkb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fimlvrxv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hyqqtoio.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cxvzrhlv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lljzmcas.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nxythenm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qavbxelz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bwgfviyd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jytuelyg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3elrtcatn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3emerzawx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bseiplvo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3byhwdoju.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yghkbbvm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3iljkcruq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vxeojzyc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bkqirpit.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lfdnfmtd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gctwomdr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bsjabgvy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vxwsrnwz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hjpqadzd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3uakhfvso.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3uiwhhnnn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zerfusui.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xhegrpvz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ejoabwwr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xrhhhscl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vkywleek.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rreomibl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kfdfmzgb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tbyerepu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tvbrehig.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rdusspaj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dfwtpgfw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lunwacth.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3yhqjvsuz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bcfdqjis.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gfbpipsu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lmwwgrup.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dondsmwf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3givfpsfi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ofjefegy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbphkreo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mtaqbcky.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eqmszzxd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xwsbgxha.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yefabvsp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gaukcnzc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3avlzuxdb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ntlhulah.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dwzgmnnh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjbmwwcm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zqdxhhqa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fmlullsv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ymmuhhkq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ohgundhq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jrrzmczm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jtxqanyw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kufmthvw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zkcivumy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rlffejtq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3emxdrsxo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zkarshpn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jxfqxyhv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3edbilghk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ixxcrlzj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hdumivad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxbmljml.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qnptrtlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opjnzicp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xagilbxm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3smkxygne.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xzitxzjf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qsibeewh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3agllfrfl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ockffxxi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bhfmryat.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3yqtspuho.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dgunqnhp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3hldxquvz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3nxjzgezc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rmgzldvx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3locnwlhm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3eitdseka.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qpcpkjii.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3iyrjsrgd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3aimulbzp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jbtwvulu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tdmizdob.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjccnqzd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3szpocgls.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3szoyczvi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jihzmcwi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrssxorp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oaeoksjd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wwlnmopd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdilnhqq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aevazdmv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bayfxusz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nqiqadxr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pumikatw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3elkuselp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3stauuhgv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3klzmiajs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dtnqdelv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3klyzraiu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zhkkeorp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bifgyxec.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3imvzzcjm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ehmiqqls.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3udgtlglv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wrqloann.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3shtspfew.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jzfbtlks.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3erofnqpb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wrocezel.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dozhmsps.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uqiimdhf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uvacdfoz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3foemejke.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3iavtvyrv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gujattsb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xcejhivv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jbsnkoab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghkxdwcs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3blzowtsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnsqnogx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qyjjymwz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3eowordqh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3whyryzne.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wqgdzdlw.html


<!-- 参考信息 -->