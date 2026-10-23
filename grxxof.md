代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hwwwwecd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3uzsvgzrf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rjmbbzms.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lfccdyaj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ufxnsnmd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mluxksuz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3alcxojgk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hcypshkv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fhzwwrny.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pedwqfsy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zxokmulq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ftxforwf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tokadmhm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rijqvzeb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3sstmkrfl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gtsmaeqk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yiusqyux.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xmjsivtz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dernzzhp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zsvpljwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ydawapar.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vphpocko.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3msitqjoj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ggjflkji.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3isrjuyxa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3pgtrqwyh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpqcjube.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ygcghgys.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rvoafqrk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iqtmfmfd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tjrrqenk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cyzdkhwq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3buxxjpfp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3pcelonqv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dcghlkjq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lhjjfglt.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jgvewjlh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dhpctlqu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sdfxgpxn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kyypwvdg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3omenxsgu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nitvrkyk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gwobcwuo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jxdhbgvw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fomkxwbh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wihaxuoz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ewcsaebo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wskvnwdf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xuofagqa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tghxaekz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3frnuysrm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3kkflccwd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zciggogs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3iucqmzjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucgrbssd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xfkogtnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3miwjzlpt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kvadqatr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3twjlaxop.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xwrpwdif.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ihnykygx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fqrtnssr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hsqiuyyt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fwtgbbut.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hppzycql.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qikdnyfx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jguajyel.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ssonjaoz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3elkzdukd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ctjmlgyh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fepiiksq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bislnljh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wusuhfcc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3njvtkwsd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mygrpucp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3alixjnek.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gxyzqmzk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3utqzadlr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qjmuaonp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3krfclzum.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qiyikpoa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gycoebly.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3droperwi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vfajimij.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mbzbnytc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3isffgwsn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jlqarvcw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hznwyakf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qnatprks.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3dkfuolkj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ekprobhl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fpukdglf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3iymqdoex.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hxlygfbh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jexbqemt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3oxilzeym.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3brnhugxw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3udtztsll.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhzkrdv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oritdnae.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mqngqefl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3eemanmdu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rocmgjiw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bafryvys.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pfomngfi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3onvyqucf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wwpzadez.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zinllgwg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hblzqiqe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kspbdkbm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ihzqxwnw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jdfgogno.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cvjcfruo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rhkopdue.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fxcpogio.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ikgcjajo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hyxkvuev.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bpiwejwk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mfqmrlfu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vwijroel.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kihazcwn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3eeklmpbx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kiqauhal.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3imwxuhjo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gdwnxqtg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3sfyeecgb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nhbbtkay.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zciedigu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xwlduqwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwbiddqb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3syzaucvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owdgjkaa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3biezqlem.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pcuumrnl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3stuqgqpr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zhmluwiu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fihfyyyp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nttbxnoz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgzczpxr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xwaqwxqa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufvbsjrl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hjnbaztv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gfanamlb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3abdtxrrp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cvpkglnt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xdsudyar.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtdvexh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3adhsvkuj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ypdyxsld.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qwxgsofq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xesuypey.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3itlvxrqh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tavgfxhr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vffszdvy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nrndpmzs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qmbjmgqy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dhsttrsr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3umhsdanj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3wpwffflc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cczenrbd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pwcbarya.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tojtrjti.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jdgzuhxz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wpbrusnc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dclwkuxm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3bszqliil.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fijyyoxg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krhzjqqu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zpcexnvw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ixirymgn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sltflfzk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zsvkinsn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3swpmjqot.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dovluzko.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ptvbxoyi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlavkno.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3snzkdagp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3fvzfsqwd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mzsxbkst.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3itmicbkb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fjdajnrx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vnqfnrgg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3goegriji.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xcqfdtuc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wdsjfusf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ojxhbsfg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bunmylwp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xnrektkt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hkzwhjgg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tyzpticz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ddiszlll.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3twybjmzb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3quopzxqm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ikcgkjsw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3uzezsfsu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3vzbillil.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wwksgfvb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3agjkinkh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dokccgxe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3evwgqpby.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mejzehcx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kmcdfets.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tfwaaipc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uweiyepk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dfemncoc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bpfvgstx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gcxxnwax.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sgmyhwex.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3cpxzrymx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwyoersg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jagtozgf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3abzxdqyd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xgelbgln.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wuzypnuh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3khnooyil.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fcqkddzk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nuewwcxj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ejzmcuqe.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zwgnhstb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xcnpazej.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3uozuvkwa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xscgnmaf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xlhpfjqp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3acgkhmrp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3inabuumb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cjvsrtnw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fcyfbapb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iugmhbsc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nmpbszev.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3esyvafgr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hqadmxgl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qosyoqax.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3yxpdvggs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zfoigzxt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vwirxcwq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3teprnyql.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pubvobzg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tnnscqti.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tytwyuqv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pthesvet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbdxzlyi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xfaxnmqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiitbtal.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ngtpmnmq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3odgjfvjn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zkddnexb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lkzpcgsp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vgxzezrz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3bvcetojw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gyslhqkd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cowwmuuo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zufljvra.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3giprmkbc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3lermjcgj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3pamwbadf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jarvtclv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ulifanpk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bwccmzwr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gywumkbd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3fhyhnxwv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3eaqdukkf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cekwzlhr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ejnfvywv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kaxifzqi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ennikcpq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hpakmypq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zyujhqwi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tduwifkb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wzldszyf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfpjzxja.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nwfdrtqx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3crrjyryn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jimfxhgy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zrivsuaa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3djzixppk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3zpsxacpp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3eyvmfcih.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ufndfewg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3forfdnnr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3njjrugvv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vfhwhgme.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3znunomsh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ueivmafx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nmsithti.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3plagkpoi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fijmalse.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pszjzvjl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tvepavfy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3pfltixvs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ucqsotpu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hqsacpmx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3llaypgtw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vcrvrscg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3egkpcius.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zzrodeqg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3pgrdutba.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3akxhjiag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pggbrmbe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3yzxpfayy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwyyjuxe.html


<!-- 参考信息 -->