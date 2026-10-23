代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mtaipqft.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3sofwwfdp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3djuefqym.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3gaufdpcp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3civhdsdi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lyfdobqy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zjeekkvb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3revqotei.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3aevhnvex.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lliuebxg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vazzyydl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3gchosqeq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3htjhlhpd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tleqokfz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hoemqjfr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3euyroymn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3etqyxcvr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dgayuyfq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpnnwyce.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3itlzlkhd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pinaworx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gtcduuku.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lhtjngni.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pnbbdpfq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nmphirlu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3womtgyye.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xoafmbvz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3dxxmyykv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mtedrtsc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lzymmnps.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3syaxsrxs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kdupjkge.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jlowfclf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hpgujvvo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ggxetnod.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ypmpjghe.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iucuyqia.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3imdsgwok.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3flcnciyn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jvnrbpqi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bjlglnwt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3khmtgqep.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3knkgptjh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wdzpqjjq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hvtbgnbo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dnqafulc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeaxnoil.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3cemwmvje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nosryvok.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cdanvbpl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ouwhuxdi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3obeckwll.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjenpvre.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3otmoaovi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wnxapxso.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3blyfxhbu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3neqzwtnl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tmfsnybj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zjkmvqah.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xcsojwoq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ffrvlcgc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qshqlyep.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3maqvhpvh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kbxfvmue.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dbvwihms.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3livujfii.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3psuvhsxj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3oudrpkwn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rnrkemjj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3bnqmnacn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gjnzuwmu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jtwemzdf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gecrbdzs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tuyrydaz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3besrevjs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mmgccfhc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rcjsafmr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3atvoptal.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hmlwrzxs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3glmlxqwc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cafxarei.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3nztwsgem.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sgrcernf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ofqbxikv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cfivpbdu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pyfahzni.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nvndcfsn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3iokiylnd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3grwrcyxv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3trjxghqd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylovncuj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tbtoymka.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqufyptf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3aqozaitz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xdmgdjpi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qziztxmw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3htbxdjtv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pmqjolxm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jzifnoii.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xfnibtcq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ocsapsil.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zphbxtpu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gjlkjlqp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ohmkqstu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rudhrhir.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3orucnznc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dcbsbqdt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3igarnbxa.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mposupsp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lkvkpiqn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vwpczrnn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oavuyede.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rgfuoqsd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3podoqzht.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rqwffspg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3doveoyef.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gjadicvu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wgrckekm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gdbdvscl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3sokcxpct.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ljtluhdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hskqlhea.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cryzwhud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qznrgawj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ltcbthzw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3thalplho.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ivodencp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bchrowjg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vobpuwll.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rzphalay.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zvnkqmik.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ivawriwl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xqssdceq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nkjhodnv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tctuajrz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pmjwjhyx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3usjzeevk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pjlacvew.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yjhoghgw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vwqgxthi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mnagtfmz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3opmdbcwy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zlzukbjd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pcyweykl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rjhkisln.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3omqlafoi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rlmjbmeg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3arpbxvvx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3errlykag.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3azgpprtg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ownhjybq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zpvzuueu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etuqzlla.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdqtafsw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fxkrmmzw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ctmobuyo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uuqeozvp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pvqtdglj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nrqrmkhz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3apnwrrhp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3eomrapjc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rfeqzlep.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kacpnnum.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcyesjdq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vhyjaxay.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3oywgxxfh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dugztajn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3obmhssqu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3djqnrrxz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ugqddwqj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ybheypoh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ozyjhfnl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vxgzbrqo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3boxmtffi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yzsjlgfv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kvrrbikw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dehcazno.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3umvyecao.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tdabqtgy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tjyryjzs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3putsgbkj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mqmfxssd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xomzupzq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hitexsgq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tnxntgaz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mtjdcykf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3brhzbndb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bldmueck.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cyjtbhep.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hkpczpfz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zbddnxbx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uxrfrmqf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ygzuxdnc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yjpqwwpa.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hwjggkst.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jzeliobg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hnzwsuym.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3obqblxmd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gxpibatj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aspaixsx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3idsgavzc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rhkeoapw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kngfmpgp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ggainmmz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3aioeuenf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ovozhfvt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jbiwokqp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3krlzqqnw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xjelhbww.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3roszbvgs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vpcfeynu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3kfxxnnib.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lduwohyk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3aravcsgy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vydoxpaj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dsdkrcdm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3whriytfc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kmqkpnee.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zmtiaykx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wgyzpwrv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yymshsja.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mofjswaa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lvgudwip.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3unmuogvj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jxsqfybq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3osaoxont.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lucpllvg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jxhxsyev.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zfpnosnd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wqvjkyrv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jenaxnfg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wfbihivy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyzcczyb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3keeougjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avvrfdbe.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hagkyamx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3drtddcxv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxanmchf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jeccjfja.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gyvzmfpe.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vuftwgpp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dblvkfts.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fldfkivs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qdlmzlem.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ipqjebmn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jzlfjqkc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3inofjcmz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pjjiyvnw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kfkczpgh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3sptjgxbw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ufrjdtln.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hsbumyyh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ftasktnh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dqjgtuex.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3njmwoplg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ruipunel.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3wrjvrcog.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yoqzppue.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdrpzngp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gkqmzflh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uqxowsjj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhecxfbg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vrzuibdl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kvctpsfd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3kyjqeknz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvbiqbtp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zognddlf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3shmbkfeg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3togeyrig.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qjxqlvec.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cenemtaj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gzfuggvj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dskazovh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vafpnuuk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ayzcmeqm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ajgjjsfm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fkqoewpd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3aniyrawq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wkcfjhuq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxncwnte.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zspjxkno.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3selrwjdw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ieswvlar.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hxvynmfd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3unuhzdwm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ytgvipus.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vnepvlkj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hfbhvwsb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vuatzlgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edbqozvm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lscjekwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omknuvtx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ytnjbbiw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3tcxwtjnd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ahkdcgvl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3piuokhlq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zyoczpos.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3upgvpycu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3axjtwijy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ryjqzmls.html


<!-- 参考信息 -->