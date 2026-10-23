代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ptwmdfmw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cyodcluy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3amhsodgw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ufptwnhu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3btnzsrqp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ucrafmdq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3cfapqxme.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qfoyejkf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3niqffoiv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zwxuresr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3kvwdhmyp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nxbouhav.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qjukiqxx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fiaqelby.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kehrugpy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dlhjzibs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xnrswhrv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jefezeek.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pkgnwufg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3lkxluzrt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uyyfuqrs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3llawmdva.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cezeayae.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hcpzqbwg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3febizygz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xrgjqrdf.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dpygtlzz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qfbeizsf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eqkhntco.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mgzdxtxt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3svfwrtfb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bmxxrfsd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nkjumkld.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ijyepfai.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zdvpyjtp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gckuilix.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xpktcmga.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mmlxarsu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ezfnaywc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vohjuhsm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3awhywerf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ortphnbl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3sjesxqwo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sjshtxcf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3agkqqmbl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dzmuwtxg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yyxdgzei.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mgbhtxio.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lkzeqdez.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3rlkimgbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsohyvar.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3obamzpnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgozzbvt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jbsnvhrk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ruaotewl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ujnblxcr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xscobhvi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3liclpmui.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kmdhqynb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gglirzym.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3gygcwdym.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mqeronjh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cfukbmix.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ztlrjkpo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kqogytta.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dztcoysn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rxvyipik.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pnugvbjd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cjintmbi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kiroekhw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zvlwuoic.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nvppmbfm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3lanwfyby.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zdttbzik.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fkregboy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3azyttxmn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3iqacdbmz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mhwboaaq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3oeukibyf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fgbgqxnf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3pjtiysqu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fvkrelel.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3bczvjpvn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wesozmod.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ocmhvcwd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3oesgyihf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rhzzswej.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zxmbqhgz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3quwvwsqw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cuuvkfxu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vclgbruv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3otolkpsj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vlpsbnpd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3glkscapa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pzbhducw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ynbfytry.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rimndqxm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3bqoqnjsa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rkmjmtwj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cnomnvst.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3aooehmcu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yczyjpbv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3atpyeesc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jgjrsqtz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pufsaarc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bvqdwugi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ntmdgdkj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mzdxyxvr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zvuscfnp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xhhpcqpm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fnzzwiob.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bjwjmkwu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lmsvvtxq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3sfuymqcg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dhvzwxzp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3twubbxdt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qtowafnl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fnztmrmf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wmqkyrnd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dwjvnnol.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3esekcysk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3inpdypwq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3svxpmytl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tctxukfu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jpxomxjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3raqxsoby.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3uazovkkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcowtghq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kgsjgkdy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyfjzgcr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vmjxprdi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hopfowzi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hbunyxmk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3upmuwvfy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dppvdyaj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3clggljtd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3waquwivz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3olwlnymh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tboqgyqn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tzuvbtuh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3psxbzory.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eahajznp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3czwrfsgk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwtugygq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lyupakba.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ulvcebyg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3eevfgvof.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kfyyohvv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dpjqxerk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kkuaxvtr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ekjyubpo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jgsqhuup.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zukzouhc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ebobtkfs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3evnvxhdq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3umhpgpnr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mongokox.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3idkjehee.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ohjibngd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krvzbdie.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zviyjvdg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ahlpakya.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3egnacuul.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nxtakxsd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pdgnjmlt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3poulipll.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyjolrgh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqonsm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnhtesbp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3umictlai.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ojdsotet.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3houdnlfa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wayuqweb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ygbmbfio.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cfdcfnmv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tduhxgeu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tvzmophs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tbddnxxt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ncsceuzt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3frkmvfmk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3utvfzqev.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sehvznyq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ufzahlbh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3inyyhwcq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qppqnwcu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dmzwouyy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3walnrkrd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xzjdkdcd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3auhndsdy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3cmwxwvqf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3iiiitgcu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rwzdernq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3masexcvb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3gprzuhbg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bbyqnolm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lcihtfnp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3soeeetyb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ezesjryh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ugcskdzs.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qkqrawmd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lpmsnjvb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3csqilgpk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jqqxxqfb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dpphzivm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rllvckdl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hpjexsym.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tivftqhv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gbixqrhs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sdgzynin.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tifkhhhn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mciizusn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3eneuzgdj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zzhqfsni.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nkvzvhqt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bemqnimk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fxyygsvp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gydraani.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnkygmvx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jshdmkma.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3hlqvhrqg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xldtrhhx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nlzazzgb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lzwicpne.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gqwhhstf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tofunytm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3wxhantoa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rutvmmgh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qcttwexa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3quomaybv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3bsmivdlt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zfhxfssc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xsmmzmih.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bergfrmc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vrxjlibr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hrwazryi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gbbqawnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iphdtqro.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vqknafdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebbsnlxe.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ifmrirmk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hqaxmpgk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dezgsany.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rlnfrqal.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uywtpetg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nmcrjkhe.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3fxgxxobt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3frmakjwf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qygwnohp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kftxpcmq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yqurqskr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qgqmyjjr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3okdtzkzm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ikckgdvi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nhrabimf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jojiupxp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3uyjasinl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ngqfrjjy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ulevhdct.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ugjhntnj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mzvehejo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qtbrlaof.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ybfzrrky.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3djrskqjr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rnkrywal.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3dldvhoba.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fwosdnvb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3chyhugdm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3unzeebjk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nvygsjft.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3miuqrisd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdpljjie.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vucjmbcx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kmrdjkci.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rkgzkedf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycfdetne.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kdggydcr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qdfrrqov.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3frxwzckn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eoharooc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xwtfagoo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cusmbkvt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3iwmkjyit.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aksosaww.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xuqmluie.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lgoqfhnq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qoqyfqam.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ilivmtkp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kcsxhmru.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xtkuqzxq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gmxtafkp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tcrmxbta.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3suorospc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jkywikaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smaxotoq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xdvrtckx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kijnymlv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3apzkdqrg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wuduoiwf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hjgjbsvk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xtwiiolg.html


<!-- 参考信息 -->