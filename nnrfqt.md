代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ynxumtma.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2czjzisal.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dasrxigr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rwiakldl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hmgepczs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vuubjbop.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sbmdmaxd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dpvjhaee.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2etbamwdf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ndccvnyi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mnvxmosz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ndxkjpme.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2nvcrpkgy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yhxfmglq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dhzvafmr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ghnqljrr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mduignmu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lrctzaya.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2twwfiqqk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xufjgcqs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hvkvqmru.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mzxxsfmz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tqhjxlkn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pvmbrcbz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2voklrvol.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ltgajyyk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bikjkpxl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hzsjsjmi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mmarutsp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2objtseox.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ypvqldlq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gqszydqc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xvcospqn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ibpoxrro.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2phputtgb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nlxelhxq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mmdzqrva.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lewhvxfd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ctfvpfgm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yvubqahx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xojycvdu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dgqynslo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ldqlalmz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mjkugoge.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dblzulhc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2cumbjuze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyoswiby.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xrcaldiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocbcupzg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eqylawha.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ywwfnddv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bflubsgt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hwnokghf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wwrdribq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mhzfueaq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vovoeiek.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2oaogicom.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rxuooajg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qhwfsxty.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vbrnxsxl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fzxjjydd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2aemqymhq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tzpuhaqw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cmikrrjy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sxcamose.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2thjbzpqq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mnejytgm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ovdqmmzz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2awpbwhpo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2grtjtpqz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ykubiwiq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fkwhnjwz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dshpanjz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uihhdlzu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hoetljkx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gzwmzwyd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qxqopezo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hpxyrcio.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2etyavtxa.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pszpmdcv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rexsuzgx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lqqvhyrd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cehgoxie.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2iwdfaojp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jtixrxfo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qxianfnn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2olajzekt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2plucbizl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rioxfcgu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnkpcvm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqzrcfu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmugblkp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ykprhpqs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cudczoup.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2isczrryl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2adkrlbut.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2confavec.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mtlcwcrc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bpkpygta.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2buqtxven.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dnlvsefu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ugkqkpwq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xfrokrsl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qfhonlxv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2smbfynpj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2eioigdtj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uwhpidcw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lrkdcaqg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qdlqsgnu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2sdwxrwhb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2yqrgearu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jplrqgnc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vowaafnm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2asykcfmr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hqwoabes.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wchpmhpp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kankxala.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lwqnnpna.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2bjdzmxtd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bnxcgpsm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tcxvslhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmubglme.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nuacefny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvzzjynj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fvnfnses.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ioqsalel.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2viwvrmox.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cgvrawbz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zrzspafn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2grhljqib.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvabnehy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gxtquwgj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kieezcfz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cskmtzyh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vzlljsza.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zovkhfih.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sqrcfpaa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tflwwdkz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hutzikkb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbbuocs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kvpsfpgy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ajhztynr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qwltvvvt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2umlbofyi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ijltkfck.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2clwxdbst.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cmaptoyw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qfroyswf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tjdpjzft.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2frbnazzj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ogkulatr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2otqdulpm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2phgldwjh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fulqydni.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2irbxynei.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqdmjxzi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dinrqohq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zygydzkh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hhjzofvc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qduinqxf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2aargasqr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2maxnwxfo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pduhzhxu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzuruscp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2idnoraxs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dkwkrtgy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hqgpsedx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zndsvwwp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixntgeur.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2klmhgjiq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fppjomtw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jeszwlhj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vgyckmxi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gwpcbjzw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wabbyljb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2fskskopx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aakizkrd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xncrlsmd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2urhdznkm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2sgkzwsuu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tznonrxz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wgmlpmkg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mlwkzdkx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2izthqttv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2mtrcjqej.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nymfesyi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2njlohaum.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jnjmpele.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xmlnevun.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ocmaqipb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zloijzgw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nvlessmg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2shejwepg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kinklqam.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dfrdskpc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zpvuuhox.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ijzszrht.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eamvmjqg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zwkoqmxe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2glpdfbsw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hzysanyn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pyxjmtqn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fryxouth.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lrlqjefx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2utilbrfq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2faiksprp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wuindzok.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rxduzydu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2bealmipa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jqnelbyj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vbyvlljh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jxugfxxs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkslpoa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2elznajhc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yfoepkyd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ozpjsnyt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lyeuvtom.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tkihugsv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kcogibeq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xhelxdsj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nkbzsgig.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ollylzpo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tdsycflw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2akxtjxtw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2sfbwcpjc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qdpztkxp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nchnplly.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pghxlvmb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2aohepvhc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vgcyuhky.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2azbtfwjb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kuzodewb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctwuyaoy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qfrjcpmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnvstxcj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2midoesci.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rkbxtmhh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hziefacr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zzhyqhfz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2twgkjtjn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dwlqhhjf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ueqsnkqf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hbkvhela.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ghgkmqmu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2meshefpj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nemapicu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ftijecsp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gzhwwfao.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gpixizsu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxajnow.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vwmjyqve.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2dwcaqusy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fqcsbcvd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2cexybrcb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gusvvaoa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2slumurtx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jorxbuzl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qoqbwaot.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaynmqau.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rpegdleo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jerqdehq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oarswluk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2eldogkav.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2qcnlrrzr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gosecquw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdabhoox.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uazpavde.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2myocngmz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2navldade.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ixrsxtev.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hptviqin.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2esssqpun.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ayzhrjhj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tsqlwllk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oacmwyjq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fosaboyv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cwxjwzfe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rvpricbt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ovipzgjb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lxspaukk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xncojsor.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2maoalxth.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2phwbapwi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ncnrtcoe.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2akaebyle.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kmoiawtc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zsndqnsh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ydsotdlo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uaounimo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyubsipq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozdwurkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppvbekvi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gnssqpps.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qevoerpx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pbeepwkv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qquvmkwx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fuqjrhsa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2exddoram.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ddxotrke.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2eaxcoovs.html


<!-- 参考信息 -->