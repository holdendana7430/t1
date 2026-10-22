代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wqlqvsbl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2wuktawst.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gqntpfdj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uekcpaqc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2srnxdeub.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ujmbpenp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rigdoyui.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2prjtdshx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2btktmusy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tdjczxzb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dvsapxii.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pnuwuyni.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2myowruup.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bcdprxla.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tulbfria.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2crvixqnt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mezyfker.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wdfkglqm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2atrektre.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jpondfjx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ygwewgcr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2khosxmee.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vwbrnecc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nkxpggey.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2owbbifgs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2snfuhxib.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xvotehey.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qtfcpfky.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2srpfavll.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xoaltivr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fwbxoqwh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sxnsfoem.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ulcgemgf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2epwswsfl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2cosnoxcj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2dwustpwv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fscklnud.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kynbbljl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tsdjztke.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kcvlfutj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hsnvrchs.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kyxffwbq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2onuhpkfj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xlfphnlv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jpwlqcbk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gaipmhnl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ofsqpjwz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lecfpcqa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bgipdbrn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gboktmqf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2abubmwmi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kwwurgok.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2isaszkzz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vdasalym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lctdxlnn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2lipwnutl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eizbgsnm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zokhahtg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2tyixzzty.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2yakqpxja.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2krsumpbv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ljbevluw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lvdzwoyu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vggafqrr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2pvqzvdad.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yfylgnqg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qpqnjerb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uaoaknvz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zislumja.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fyhjtixa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bcuqkqkf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2atpxbhee.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wchezrgp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2frhmsecz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dhckeuqc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ltbkchdy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cryryzvp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bhudvekq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iaytozyg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2psltfdfr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lrtxlkxo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nuzgmcms.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tsfbyfyr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ukobcogz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2betloihy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lflbgtjg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2etbyjdza.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jdsgkzfw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dkjxerzh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bpzaituq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fuahgiev.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rnfyxjmh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2idaltibb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mqiduepf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxygplmm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gfyhbmky.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2baxhthbq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pyclxphd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ccjzfgzk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2relgfqvo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zmvbixuc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nkfyjipo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mmygrnws.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvpmbnar.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtnvkf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sovcvxvr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gabiqxer.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kqwmgygx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ocdefumz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rzkzeqoq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2miftjxsb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cdamdwnr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sfeyjmsk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sinskkfk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hzuhotlp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ncckgtov.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wwunmaay.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ieifnsid.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zlkrdqss.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iubvhawe.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lqlkgvsp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rqgifiba.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lyaxskda.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vrnbhzut.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2shqgviso.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2iqetvjhe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2omsidgbt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2trssfzuk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bxzwuqka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clrzuiko.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2syfnijix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lypesfie.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dfxikpmf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqarmowu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uejzwynz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2areswkny.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kgeqnabg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hfbbsepv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmabsjsh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ttpmjrem.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2widxfrsp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qbxeqzzz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hjyruojm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wbygqiqf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ybwwvaws.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cnsdljlr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ygnjndhq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cjywyqwc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vrhaecqo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sjehfggf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2airnnqik.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pocuirch.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jjjdrdhb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2doxsnwzb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gjuzgftt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nddqtsid.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xjlbgdgl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ndgwwilq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zjbnwhba.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ohwfhcpo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxlkfthy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbmlcrek.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ycakktvq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wccxmvyp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zjjggwad.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zuwvdlbn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tghkxfuq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2aorpzsgd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jbzhqttp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eerericv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2iuxbdvzv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qpchrbwi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2thmkcqso.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ayjmhosc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2macsfiqi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nakdibqg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rgnjjaxv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lsqkiqxm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2umbxkkaj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jexmbqpu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xwcfjdji.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cxclomxi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wtvltagh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2crbesnvw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cdtcwbdc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cohhdjsb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ozsxvuyr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gqwfiglz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2aisedepv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mwumnqpl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pspuolkg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2xpzsoaof.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nlpadpil.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ykhlzghr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lwkqvmey.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2nlplfqlj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwotyjh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vaskezdv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2orvvkdek.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2paebahzb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fcdbvmgu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pfawrtgu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vrxbqkyf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ytztgixm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtsmqbrb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pysbxpiu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jesfsdpi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lubrmnfb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2peavyrwh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2opkxdlxo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nqqhpbkv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kmtvitsb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rmqhxxzi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ikuxibfy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2alydydhf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfghzzch.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lpxxktio.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yitisgid.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwbiqbuy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pztmbums.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vkpqxwfa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wfvdxnmo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hesowscr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2oxlvragj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2iquqodry.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2doevjztd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jdbahlnm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xwswwekp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rysviynf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jxajdkjq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tqvocoxq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fkhsroko.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tjvwrtah.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dujqqhkk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mvxxgjsc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vjrjljyj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gvusgogm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kcssigep.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qtatmowv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fqnhuojo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulkjlqdz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kottymah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jaensfpc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lzbxwkur.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dwbccryj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qhupuhao.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2zobjvvbj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2znavyswb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hdxvtnll.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nodtwqrw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jqpvprxg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gelsokmi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wpjfytnb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pjrbpgrs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nfvmdmok.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2czwklree.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hwygpoeh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cehixehb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2jxvircer.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uuoxvfml.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tfvdnotn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bpqvjlby.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2urkaxfkv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bnildfoo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2fppquzbd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xnysknpm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdunhyez.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zvzjpxgs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2szsnhpgo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tvxpvzvi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ocmplnfg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ubcoxlcn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nnxvladd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffkhsgxb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpxcopjc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jxdafjwt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jwjwqstd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vazizoer.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciyrjozv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2gxrhinag.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2usfqagnz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ftuvgmys.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qxvcrfau.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhhjadr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mkauzbet.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jjkaypzl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uypndpie.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fabwkbrl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ltxbexdg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2budhwclb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2gesumbni.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ljluynju.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2stqejtgk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2yahiyhrf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2zhjimafs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2riwsuweu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lbkexfor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvhvblkw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ksknesbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkdbjcyr.html


<!-- 参考信息 -->