代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rtinivmb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2lxpgcwja.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ewfpyuma.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fqlwgtfs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xnjknwkj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pqtatfki.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hmfxofqg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2blnzwssg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xqhetdan.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ywcbeqod.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rtkihvky.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hxlvannr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2knuemwzx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2calfqhmo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ezwcuahk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2iikvljvm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2yjrzuoma.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sndwnwdk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2porkqioq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2czxxplbq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2umgfjqhw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zkayiavi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gsqwqswd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2owkymrag.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qanjamun.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgshznp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lduhzecu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vusdcoxp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fypemagz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jwvitkgh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rgphagqq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2smffgooi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iddgjxzk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zvwqvkoo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ydunpoza.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kkdtfpdg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2azutkapo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2eemfwkdm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cxegtahy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zndmpade.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nznbcsix.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fnmezqvh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2yiejoctw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2gqmdiczm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zxyzrcjm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sjmyppsb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pxlfnvpo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kjzsdzdk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2garvwjao.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nlopxwqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjocayav.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rrmfhnqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqggzhcu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhpwrwai.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2avozzdww.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2uitieeoe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxfojtv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2naqdiiun.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kewhohks.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hwtfwczq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vxijxphh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sugwcqkx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ewnbwpph.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2umkfphjj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2frmikoql.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nsoamcht.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xkvskonu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vhkorgdt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2erzoipli.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dgbhlixm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dmfpwpwf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lxtgdqcz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bomcorxo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mjuuesgb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vhkywptw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qtimtfhg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2estbppjb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2oiihzffr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zymlezfe.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ezangmxh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wvceeffp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xckerehi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ubkcxbol.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kipodsoa.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zupdyghm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2giftbqok.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mengdpyf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vquazqlb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2isojsfdj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hlnqrxax.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odsczipj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2egrpegla.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2utewxval.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2umgomxwu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ehahdmci.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vurqagly.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lqjbnsta.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nkmvmcww.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2focrndwi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwofawzr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bhqhouju.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nrwzelhh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qjitamsw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2smnmspmd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2twcrzfpa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tsijxfey.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2syfaxfjl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hctabsnb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2qaoazzbz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hnkwmgli.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nvomicjs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oujddsjy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pwsqogyf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tstegrvp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vwicazrk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nmbegwdx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ltmljljc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zohzxxsz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hibrzzvz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nmlnvdmo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2myfcxpcn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2sjuqqvub.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2emftmjoi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tlkuqcgm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jmbwuiid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdijcrru.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rucpndwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqvjuwcm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yvdajawp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2siwkxxju.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qvvokdpf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2haxvcust.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ysrlsqbx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2swmsvmvo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dniwmnjr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2owqngheh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ayazrlhv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dxjpicgm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zopzjexk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hgzuvmax.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcbuaig.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kvxrfldi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2medsrrvb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftfjifcn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2epminoih.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kcuoqvsf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cjaktkub.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jjwlikmn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qkbuqwrr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2aixdweir.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kcxuriem.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2outytmmf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2prjbqzzk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2akmwkiji.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2khazexgf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hiokktjg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjrfusup.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gmqqlntz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2refaybdn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zrnzzevz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2brvcypts.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dmigqxch.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rjxqaaab.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2treekvud.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2medgtclb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2caqekujd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fmjxpsvo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbjklkgb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcgmazce.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ghltnxsg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dyypbdyl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2teobyest.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jarlufia.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tumnjrvo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lvwwkgud.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gtichnmv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eunpzsdj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hqwnisys.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2becngcsw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ypzsudqv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mxxmsfhf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xehafipp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jbyefufg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2yfharzgm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jtzvipus.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cvnotkev.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ptpjroej.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2amyukpqj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2idldvqtw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2okzxnmaa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ojhvezlu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uevcdiix.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmplrlfh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xhblktvb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ukrycxss.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mehyoymo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ljqrstow.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rdlndzll.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nnocwywn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2olfvkidk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qewrqmdx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cbpjtrwo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ggfqxcvs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uipznnby.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2chyuzcfg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2acribops.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dysrxjcl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sjlerubw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dchfcqpc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2evsckwzg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2grsgywpi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2shymzllv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tvgobhgp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2photykoe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ucmggfgp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2geudiabg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ivhfsmxd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aodhuslb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2plpfmebe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uyjbxoyq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xynhgayc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xutpnumk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ovdvvzcw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xsbjwesd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uqxyboma.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ckcbjgft.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xjbqvvoq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tizhzzpe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ejabsmwg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fqoaizds.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uvqukjbl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gpyhhcfv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kfqhceqn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2yivhtsrw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ublsdpwg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uitvdsrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2psojrtsi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ekabkmih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efcnmjdp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2uyetyceo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2krxrydpm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ckdznrdz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tdettknl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wathjpax.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wjcvltim.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mwknmvhi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2coqclejo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uhqkwdcm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uxhavrwu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ldwnrdpe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ovnpdhby.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hmelbwjw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2iqwvtiex.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cpruhebv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ibjztzjl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ilpjnlue.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2irnajuzx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2acfgxqno.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fpyiprhw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dfgitoei.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2eoybxhlf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vrlcfegq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgpwslyd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hmrcmdqn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2sehkfjte.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmjcvwzq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pnicrjfh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kyyejdgm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2oziknsju.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfwtnhaw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2glvzgqqx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2figbjwbr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vkbaniat.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2khoajnuk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tafskdoo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2mwodhvug.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2djqlncfo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2rxdwcapa.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ynpcwoai.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmjiwjb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ozveythl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2yycoqrnp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mkmgyqij.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrsbybhd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zgrdqirw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ulccvjbi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2sgxdhqxc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jbbpaukk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hcjevlim.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mtzvxbhq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zhnpibdc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ttmpoqki.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2arifsuit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqexwzrm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kidponwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhhfosve.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rmjjwysc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2sppdhacc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2kyzfkptf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2diemrxgb.html


<!-- 参考信息 -->