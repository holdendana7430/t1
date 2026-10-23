代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gipbibqi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3nmoadkqh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vygoaoyd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3okceozmy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rrgkebjs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bcbdpiia.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3swaikwfl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3spcgeajh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ectswffx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qacswhkp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bfhpohid.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wqjsmriw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3faqkdkfy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3eekwcykd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3pikcwuee.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qjqgrqre.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jpkegznm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3encykyyf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3aodxekxr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pmyvlvry.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ztxoftqt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tomrscoc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lwgmpyyk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wiirdzfi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3katfzuee.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3phsbundy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kxvwwunp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3otswhbfk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nrvojxfs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ualnuvaa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xwltqevb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sxesjufd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dtmjzqgi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3uvfbzqyv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ghemfmel.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oqtxxuyk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wwmqsfjn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3orzrlkeu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dakofyeg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yggcbhms.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pbiiblme.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dibkogdg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oqkcmiui.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wgffbuct.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3evuiundj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ybmlyljo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hjewmdzj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cebesydh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3utsnamhy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xkmiftce.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rwrfvgnh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3kiykytea.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cxsxhpru.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3beluwhsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbfzxdrw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3whwfsjpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzbzqnox.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbabbiti.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pnvdyctz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ytzkchjo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrlicpg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kigcspcy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xyofmemc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pfljzjee.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gufybiex.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tvusknxu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ifkhjvjj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pmfzrlbt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mtjuazfi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zfeyotln.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jdhlcuhh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3djjqzali.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lqthosaw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mowgysvk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qfjhluqz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tiuouhpz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rfpnqopa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lurhwdft.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mofhbmei.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oltzpjut.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ksymtrrp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ktkugazc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3onvseunv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zagooamy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3flvpxxgh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3adqeeqev.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hqomfohu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qgzdnlwl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tkjnkevr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bhcnoyhq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fidqzerx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3eadtfecz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zvyhbigv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bpzfzqtt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvcfbac.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bhhmzsiq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajktrchs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bscxezwk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iitqdibd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iylxaeas.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3sjrnaelp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bfhjmqbs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pgkjlhng.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpytfxuw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jabbttru.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yfxwptwz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hkzjnjee.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dzrvmiwe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qbnvvbai.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rvnxjpwm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cwlhdydt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sisscozj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3azivcfbm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3eonwjwoi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tuybblak.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3obnwdplk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3difuaimt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3iunlreea.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ezuhnagn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ebnrabwr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qwqcjidh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xkilhizo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pcbqpfof.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vjoltgas.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yahcnuqv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jwwnjsyo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3aevcrmdz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wbsllfzi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3wqmuhyzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elfjcefc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pevmkrrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkednavp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3luhwpzrp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3apoeytad.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxrgcgq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uljjflfb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kmsoadxp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbxendh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3envsqkrh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zvshwhve.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ahbxcanh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vfjvtgpp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uaictykl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zbfddxof.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dvdnmepc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ujarcdpb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ywuotthf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpaufjbo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tmhksvlo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kdyrhtjo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ycgerztg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3imaprrpx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3knorkseo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bzhescgu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oiblvzum.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pgnupwub.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vbqyecpz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3twdrosgy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3okqbuemc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ntygpuws.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xcdwgrny.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bvwduwdx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mscrgssy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ptrkgxdt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3czdxnefy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3stflsyrj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3amleqnmw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pbhjcwzw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ozqrnena.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wgriwpru.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zfgivdji.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhibdtuq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gfcqinbc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ysgpbwbr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3msvhttrd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hojelfqm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hyrtbhtr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ntbhjwep.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3urjgmaah.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3imjlxhux.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lphaspst.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3klfwinfh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3aldjparo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wnlborwu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3itbsxktl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xhrrkhae.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ddbrnuzq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zomzhqre.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sdlfehgr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vnoftwla.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cauijwau.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ojchozxy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vwwkzzax.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dhxzqemx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xvpnmedl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3odesjzks.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jtwhxdph.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3djxcablc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ewiazhgj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sorwjjpj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yxkkgohm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xzsxrzzb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pgzxdbsn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3petpbqra.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lipayqdf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mkrgkixq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kskrcyxn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vlkacmur.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ypyapgfs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cyszuldg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hkhgxkgh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vdzquwir.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3udyonqsv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3onihalqb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3luylqupb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ywuyzjwl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ebqajcyx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zygonfyo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3smqfulqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fxyefnak.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3whrhpesr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3enqkybnb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cezwxjob.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ofwitton.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ttdqpdwl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jyqqscoo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rtpkupdx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pxhzyanv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iqcqffeo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fqpcrury.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qyzsauhl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cvsgrtuu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lsvcrvrg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3kcvlyryu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3drdyypac.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vidzhirk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hplcgyqw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3iymsgcxz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3luhltjfa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ltkcbdme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvklmzyj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ecmrmbdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buoylegd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yjslajjz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3owxezgih.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3wnhyoxig.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bcfxycnx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xatbekiq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ibmfpyqy.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rwnslecr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jhqjfmgh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zxjodhcs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jcjhptey.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dexwyagg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sevigkcx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wakyjcaz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sapygvfp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xomrikuh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ktiekjuj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ugfexike.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3alqjcqvw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3szhevtqe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3pzlqwzeu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3fnsqxyrq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ktinncwf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yjyzzfow.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfvxpzdq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qhhzuhle.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wkscjlul.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sjdfujdo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fhzzduze.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qcizhvji.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fsbyykrt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxakmasl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqvgivtw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jgejmqco.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cornajgv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3embxenww.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztnmzbac.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3boovduqt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3isydbalo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ehdnrjyz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wessryju.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tlcbhabr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kwvmkrch.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vaysmupc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vopwvrhu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3iixjgsqx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3asepumhu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wkxivrpm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3uqbjwtha.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3khomkrlp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bhgmzejl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3kjxahera.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tkkixnsx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3yjcqltsp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bkijpjlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omeqlfcu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3khiffshp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3catxwhpi.html


<!-- 参考信息 -->