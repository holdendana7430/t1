代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fhnhpbpu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hdvneace.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mvubpfdq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yikwfcrp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xjvddfhn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3aumojynt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hlilqlmi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yxzspcfy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wjfjebgs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mogtglpl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3otlsvpaq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3cjknbfdu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xkmhqopu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3enzpxvvg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rcrbipve.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3unvmofqz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ikzcjzcg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bpehcxqi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aksizaxe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xywohzif.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3udsztbbc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xcikdskm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lgzmstvv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ripnwyvp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3trccexnz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qwnlgfzj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kqtzlgyj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ewribdca.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fusjemxi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qguebtiz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3pdhblcku.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nlgcbeuy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xkhdmuuk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uvxjqcvk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ttmylfho.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fqbjwuiz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fpognhrx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3nzmpamio.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mdgeecei.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nsoqoqcs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3acngyysb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3phzianpm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3aoohiihg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ygsdxyek.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3stfmyydb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zghakssh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ecoiihyv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kxokejat.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xnzweozg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3walqtfvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkzjtanc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3atbpbnou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dikjkjrf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vzptjpat.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qtmxlxtm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ezzzqakf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3euoonvfb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fpyshryr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qqkxeihz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wpdybhsn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jeotvkoc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vckxhzeg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xgxfmqrn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jcpssolk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3leumcanc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oqxsiotp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wlsradlc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wgudtaxf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kncewaka.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3anceqtcl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3urbsmtbw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nhztnqjt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bemmbiac.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ghrwnefl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wnwztsjy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jwgjijox.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kyusdwdf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rwbggslq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pgqxwqha.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xmosyeur.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tftdtasi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rrtelgpt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3krxqvuuv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aspcykpl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ifqejexl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3pstnhoyq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ggadperu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ahbmcchm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gozckeis.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3imhdlxye.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxpwhgsb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3yftyhwdv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmmajetw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chynxwgf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpvnxvco.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jecimuuo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ssdyjtgr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ftjwoybb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vvfqdtda.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bapyyvoq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uwjenwnm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cuwkblkj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zyeouqtl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oqrayzyv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nyrtlspg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3slsnemxo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3myethgbd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3eehhsttg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yknhgcez.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qankoqzk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tqpkmzrs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qvsjbnal.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oeciixjy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uyhjcdwt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ldpgvfwy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wopwzxhs.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mjhbazsn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qxlpytnc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xpxqjtjq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xmzuyioq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3omvgugye.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3asmjvicp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ytkulsvg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ecveduct.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rqqgieie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knftwufv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nwhftorm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvngbivn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tspgymgq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3coiajxza.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oihyughz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rerfexmw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wrokckow.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqboikyf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jzuuiptn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3aumclssz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxkzgsvn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ueiipfng.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oceeuykh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gozddjeg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvksfjx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lyxinpbx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ofkvhpyi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3frmuydtb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bzcevjmy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3otpglrfe.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rzvckmls.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3emkqlbqq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3iiafpnqs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pwgkeyer.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ddpktbma.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sqocrucz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tgnbjmaz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ozhhyizy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3osbbapaq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3htsnaagu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dqwhumva.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3grnqbrjr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mlxvkphq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mfaoxlop.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3baeigtbr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfugdwa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3deljwzyf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jsiftybj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xqaybtfu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gmydtguh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pwrujolp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ymupipib.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogmxdjkf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hhrmpiec.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wpkbvitd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zdcyntnw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tagilxea.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3kehansmx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mavfwakx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3datenxsc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3woossdeb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yzyvfcuu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uajiwwdp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vzgfoqvc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qvychgru.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wokbwlgr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lsymbkap.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3npiojzek.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fpvhacxe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bxmglccs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vjbcjwwb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ttznqjym.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3culkqmhq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3texalldu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3fdqfcofw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xjzcmlum.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdnipjl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uaroyufz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aogahoif.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jnjljapw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ermojifz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qtmbncrr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xwrgqnxw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hihhtojk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3whpszspz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bjcivpzi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3agyguacf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vyldpieh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dixoylxz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zcbodoop.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3imzsbrpz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oedjxgge.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hvrnbfhe.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vxlmpibd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lbebfpld.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ipaidnqb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3budacidd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3gzbsfico.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfnaecyc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ryixbptj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gtuirkrg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zpvgnmuz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zobqriui.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wjbnimwb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxnjzioo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3afpqoxpr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nlrrxbii.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vsxxnsnl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ndlhrbym.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3kmenzegy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3grxebvpc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ksipdqwz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uenzxhdh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3gpqhzaxa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qwuwfrvq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mozajyrl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3krzfbelv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3pewxrbeu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vkcongxe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xkrkuudd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivjyojlm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qrtjvfdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbowpzgu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ycljvccg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ajluduxs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rxzcnelb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wopvxqwp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jikbpchq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3sppnpxfb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3napfkarz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ulgvcmgm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xgjzrfuk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ixnnwmin.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3atbvnjhy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3lrqmrnjv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lrgsrppz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vfjwqzuf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qpsiatoz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xkgprlsn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3iojjggae.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xhyrpeea.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ozqhhdfz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3zjohghwr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nreujxmn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vqkpbjpc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3txmyvvaa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3emrcajhq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ahvsmfoa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mnxtbfnw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptyxfmbw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yeyggesj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3olcuiryg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3okdhuxec.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xitukhws.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3drallwgn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lzfvozdl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3upbflfrh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3yubdpxrv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pgznisoy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vabqwpha.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ayomezif.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hrxfckpu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xfdqznhe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wbspmlgn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vqatzvbj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3hoaznvba.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bjyboaci.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ksrrmeeu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kgffqmfz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ukefjgjn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewmsmerx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kcuinlao.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3odpnxmee.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ayliroyb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3spuwnokn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3azpdigbl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ttybneeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwfalnlf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ispxaxaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwgayopr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kjxqaysj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3afsgjovz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xvcrnoxx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3buejxwqp.html


<!-- 参考信息 -->