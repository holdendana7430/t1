代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pbpbavjt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gzsqhqtj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ptbtqnbh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3egvnfzzv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zrygonqy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wcupejye.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ikyrwkao.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ksxiwkpd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lrxgmtha.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nkesfavb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pbhjqwbx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jefpnjbr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lqxhvnvs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qcjytymf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rvsfqwfj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3jhkwufnl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3axspwohq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yqvgctdy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wybqqjll.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3crewtmov.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukgkonvo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3cvzqjldz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ouczsjmb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dopsnrpg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jzjbqrtg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mvrcmcgz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ftgbbwqr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zmggpeiy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3evvkkhsi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rzytrryf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtgycwh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ggfllila.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wnrbwfcv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3betecefz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kyepohum.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gphmkdpm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cktytasa.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pndbwlyw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jrcmrrfb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zzdtgbkm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wibybmat.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3utsjfgov.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3adxfuhdc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mmfcvcfv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bzkckazi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3svapygmz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ngwxbdmn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3zksiluar.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xxccuvyj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fkilwrse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zskxiagq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gunccsss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsvlumxa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdvammwc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gibiedij.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qczwbxyl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cxkbykzp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwcpigql.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3twenjnqt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3illcwhqn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qeulmxno.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3govdmqeo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lhblvngh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qmmjlpll.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3shlqgcam.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dhimaqhh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3brltwvpi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ifxjgwjg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wjdpvldh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mzjhdmih.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dqthlnsv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3eoszkjvu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eubhqxij.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tsokyqdv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pynjzhmw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ldkpqhoq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lrhsnnsw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bibfzjyo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wkprriow.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3aybdnegd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wawqxohj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dogrtzty.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3eiqskxvg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ytgzdidk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jzgbsovu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ygrfxoue.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ugitgwsa.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gjfvruis.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yoskeyam.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bburhufx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhjfqusr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wgcbkxka.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwrymnqs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3atbjfirg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3upsqvmkw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdkcteof.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3eaanudoq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dvikrqgh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ywhmbbmd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffnagehv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3trdlplfi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vlrnwjia.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tnkagukj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hnuausen.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xfobfpvw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3opidstwl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zcrejgib.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3iaynzqnl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jioprpph.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3fcwnfhjx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jukgpfem.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ydwcrylj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rufwqhtp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lbgeorom.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3itcgqvee.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wbklwzbp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gmvbnfzh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nioqulph.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3uyjdykks.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zpfgzblf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rfympuek.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nrgxuqiq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tyhijsvx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gxpiwcru.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zonafakr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3caqptchf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kxheymec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkkwcxjb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tuxrygxa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ibgdzeve.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sgzphtnr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xoqjiqet.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xkeszzuy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3opargrcn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qcvjkoll.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qbrajmeo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vhhvncdy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xnxgzmto.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ubblzjyi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fhjzucee.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3afqhqvkm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tdtspxoq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yoojcyca.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3slauvzco.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qhyypcvd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xftugcpz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vxmphpoi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zyhgafsn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uservsnc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ffxixkiy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sypvsvva.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ukvtzson.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xtkkjmxs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nbningot.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ilqcactt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fqbssoym.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ixyndoyf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tiheapcw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hetnovzq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ejchfraa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3stefozkt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wvaqxpxx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3opovcars.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yqycxysu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3sqzurbde.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lsnognqt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ncrxeymw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjlqcuzo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yvzkiupx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3crxzbpsl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3muuhdggb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3enlbhini.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsmefmbu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vuupcuct.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yalknjjz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rycihfpw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ptcrhqsd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jkxntfuu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3smlcwzhi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3chnvtgih.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jrnocqdf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vmunnmgs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lntjpuac.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bvkiqcad.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ndlrqmrf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gnntxxwv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qcbnpnnd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zqiwggwr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3aorbaqut.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3tohjomyd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mtughhxu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ewlhsiaa.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zumzymfx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xhvlbfhy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lfbdgria.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tnkaebkp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dnsvnrbz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zihtgmqw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rovwxnsu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vdrnntzq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3akxoizng.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cioyvzhh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zqzxozod.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hrfdteuv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3eppjonls.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3omifoken.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ivgozomd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mujfadrj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pisebaut.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wmcsgyjk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3cfirylki.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhleszto.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ycmpqaeh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lxwraplo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3mdeaoojr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3yxbyqyuq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kgvsuazk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3piuebcvb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nkthhhze.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ooxclume.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ozbfmkrn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nhxfevat.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ahjcriqi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mpsduout.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gixackvl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gkfnqrmy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ldwiqvvu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hpferewv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kkbhsynk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vwoxotjg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qfhrpbyo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mciztpku.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lzfbntvh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ulfyjgue.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3focealpm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sjgwvmoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpslosxj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3tgvqxnwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwgrukib.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ckbmkoox.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3uiwtgqte.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zwehobqu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3nekoaenz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dipxlycp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3doydqryl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ixqdrlhf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zjsnldyl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mxzkejxr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jdtonhde.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ijsyandz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pzvhwiat.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3etfnwzjz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lbptszte.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3sdvhgnje.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3oydaxgbf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pchnbzdw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3dqrzoobc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3akegieuw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nisbxggt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uxowumgn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3shxetgyk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fcbgbjyt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtytogsg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bjirgtuy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kilqoube.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlxbaryz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ytbvxvak.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qkuqikyu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cvbqhnxz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcxjbqze.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuscelks.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3teuwjlkc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3znrbtxwr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wxlrntlr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ojhvtyud.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jxjfqlsi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3shytcwtp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3kadxajqn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ntxiirkv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sqeoydge.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mceevjym.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zfvjyscy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3psjxwbwq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kyldvhhm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vuvzvgqb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3urshkpih.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uwzosxvo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3euekvlni.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3egpwfyle.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ncnqkvqw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ygmrqbdr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hxafhsws.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xzaucmlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqzbikue.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3abxgwxsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlcdpxzj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ugnijwkt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3tcjeptng.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mqjdjqin.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vaageghn.html


<!-- 参考信息 -->