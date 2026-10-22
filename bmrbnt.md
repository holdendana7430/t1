代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qpkucmpe.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2fvbkingo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2qeiunpem.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bktoikmb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ewiyzuxk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fxksmjnj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oootxshb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vixtgszk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2tolulnai.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2erkbzkud.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rivvhqxn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yteurrgv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ujyoracl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wrpcfkgw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sncmpzgq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2davjlwht.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2lhskkjps.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lxfqdwum.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ciqtbpbi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2anuvoqiv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jekgdurb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hgdocmxg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ioezqeda.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wbzyhfle.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lcsuxvxb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2idavdkmk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tpumgxij.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dsaepimc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ydultgph.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ohoebswn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ggizlumu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dnzupitg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2juzgkoqc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vehroyfl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hxnjhqdx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2crbkltfi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qrnmeoop.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kztfikum.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ulbiboji.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rnornbit.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zhnlmsic.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tuxkbbrk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2csxoybej.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2msgocwpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rptywdbq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tjwltthp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylqnlzws.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ozohubmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btjxjmee.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gghblite.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2aktdovww.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nkgazjue.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pglbwnce.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qgfcjvfb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jgkqexww.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bwpidifc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gztdisne.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qwjmdets.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zvhidzks.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wtvhwzlx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dndrfkgo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cezbtqjl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2unvlbsxc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zpxkxdlb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ontflaqt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jvpllyjj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gmicqtno.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2pkfkvyrh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cplwdgoa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2oyulyuws.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yoamfmjd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dgooblxx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2deearjgg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vgdyfnht.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cebsbhxn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jqihtrcw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2alsjmnrd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vjcpuqwa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wyxvmims.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gkgfuohj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ghhffrlp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dfkhecwk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bxhasqfd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2enuizecs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hkqojkem.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xcdofaff.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2omkobouk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uihcvwrb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oojvqfea.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tjjhzyfv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qanpbtmd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kxnqshdu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2phqptqup.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pokhpgsw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tmobgvih.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ybovlmnu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vsfhjcun.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nvfznqwa.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2klobcxvp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zyxguxdg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2didnjmfx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nlrxswra.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rmpjnsmc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jnfousnm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gcodbayb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xpoaupcu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dbajomji.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dnknuera.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xexjwjju.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2nrydefsl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lqwelbqv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2sxeithew.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lrivszhw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2siksvbjx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vnuipsna.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2avuoxyaa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jimpmoje.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ewbgzubq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wqdllgjr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nugrcvty.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2fafmqegb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eixjqluh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2glhepvgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzwjopcy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2sjuhssvn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oocegmmi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2llvsjxgy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2clbidiyp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ozqpsjvv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aqfskmnh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kkfgmakz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zhefgmpv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ujduaqih.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lokbcgtm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nwjynajz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zeguashl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2drbkxaip.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xddbbemu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cgebvllg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aizgvdjs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2klepxiyi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xhvgfixu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2poyleuev.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bsejpbtn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2smldymue.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gkecegcs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uihlxicb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gktctmlp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bmfyasuy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uyqbgcgq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2uplmahpo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zbelwvhn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tuhnaqig.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oivrhxqw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2erejnfec.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2toiolsrd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2riwfhuxo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dexjedgt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2arkrrlmh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dwlfcuno.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ewcdcazd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vwgcehzq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhmsqbbl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2davydcsq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlpqzqx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2aimkllqn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nkhknelv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2laztagku.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdawyang.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jkecfiip.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pckwotcv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lgfznrib.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2amischmt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rymjalhm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gmcprnst.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wuqrunno.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jgomwkvn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gkcdupmv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ftmjrkvl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bhoritmr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rvujbcpu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tczwmvif.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bkbpsbnt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kakdjqkl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ervbwena.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vnltnmlc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lvdtqzsm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2sorvvzqc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2skcpjogr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vesbbnrr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mdwdgnlv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ughqwcjg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eaoxjebd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tmcrgpqg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hndhqvhb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ypcgatto.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yuhfhhci.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wziymrli.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xsvdolbg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2srwhsqia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cbalobas.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2encubibd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ywnbnilf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2okxzwvqk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2txwucgpn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tgypqxwc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rgmbknsy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2njsaxfru.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yxjicwdc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kbdbnvfe.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxemiwu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ptxlscso.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rciflwjb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gskoccpc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ueukskov.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dfprhwuc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jghmakmw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fqiwugjk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rxugxpmj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2knsvhcgt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ridesrpb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rkghdubf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2umgtwfna.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bjsztfkr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fjgoejrt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2witzjzui.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yywkeudj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kcwadtbc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wxdoekbu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2prkyaumf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2govddawz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2krisfilg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kimatsfh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kzvswtmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzzkpxlu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fupgxwyt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hsmflzzz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vximxfui.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vkmuulzo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ounbfjpc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lewtbtlk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jcrxqfgd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gbnuadwl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jivdvoqx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zelkcaag.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xcdkpkfh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tfpzvgfh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2azzvslwf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rpbshglt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tbpmsbyg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mlitmwwn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2unkcavba.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wqdlvpce.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2uxrrxobh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2agokaywq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gtpvmjmn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2lhdmpdgj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ljuuyrvo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzijzzgp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2powpsshx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qtoswzos.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2erpthssd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lnjnvbbb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pjybdvng.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wiuitizm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzrtcici.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cgpmzvuj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2osbgztcc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2horsmuyc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kljpgdlt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mdvdrgmg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ubpihufc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yaryduvz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sqtntzus.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2efzajmkj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrvskzr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2aduttmlq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2naufdvow.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gqhfwhyr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2uklcyoqc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gljpbyli.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fxbinxrj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rcwpdejq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qrbgkwff.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tltansbf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wxutlkfg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lcmnlcgd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2maaelzus.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xhvtpeyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyszgnap.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hzvjsswb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojmiugpe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yotyhsaw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fpyorgvk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lcogrwyh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yqlbfmyg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pgftmrob.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jdgqjfka.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2uliqlgxk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cinrfmjq.html


<!-- 参考信息 -->