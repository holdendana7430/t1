代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vimfultq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ussyokme.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kbyprccn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2caipjhsm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lazhlihb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zgunhdtd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2nrehmkhm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ibdfwino.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2unckgenp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kurupkwc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2refkpvvs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vjonfwdx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2avrkfxyg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bwtdojqr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2nydmlnar.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rcvqerjp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fqsjmjuy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pvifkndb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2mvzdvcll.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2msybvxxr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2egvxwmvl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uetvilvl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rshaufqr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gitmgpaj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2iwajdexv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rdbizksh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ayxpipvn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2trubafkc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2aczyoeyy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ehvskhht.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jumricgj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kwhxqyzj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2spiazdix.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ymhkjynd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cxyzqxxu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zucqpjta.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vhwrnabz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nutfzgiw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdgphnw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vagsgstf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qnxrunky.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ofxveryx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2llmlkzao.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pkjgufte.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2whavqyrg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2exgmufkk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yhsjggtq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ndqgbjja.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yktamsmr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vubrdqeh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bgogbcsf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fdbynjak.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kbjjeqwh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uddxekqg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2cwarxgaj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lemchvfz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jfoptchu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tiqzehdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blxixkpb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2nhyqfgsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slxsslel.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2alufrgat.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hitsielt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2sjgcftco.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2akekyeqm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cxrfmpwt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zjtsuxqj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cztebdqv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fotodtik.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jnqeipbr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mzpgbahi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ofledfpn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oqhryznn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ekimnjdg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2akzztvhi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qbphlofn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lqavqiyh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nxtsylfv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vahlwfor.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ltycoimm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yewyuczc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kjjqwxar.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2shzylyfc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ovragrvc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2aoaplpwn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2prkrzboo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dhboiqmd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ivblfuhm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2olfzcuec.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2afeasfcf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cevbtmnk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bkqpltai.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2epbnbibc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2etxsjjri.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qlaffxhc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qrvnmhco.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2hcbyzfgx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yvcpmsom.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qepkkvww.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qvjrqyza.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxtlojn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zknzuqal.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ctzohcou.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqrognx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xownbigj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wudhxiff.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xlxwbqon.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbnogukx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zzyizypy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ouycpepv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nhfyfqdt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2agfhrsvf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wdauznkg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2clzqaalx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2phendayj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2omjduwlf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ztkfiyzf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mikizspu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2iljaobja.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nonfryfy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fuxrhswt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tjbmqrqz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gtrxqvvg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rhltuckf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tgfxudpb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2gfngftqx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hdlzrzyo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gxcfdafy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zxmgualh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2saqztaxv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fkqgnmfz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2sgvecgla.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2atinlscq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qihydyxa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2imojqoyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cazbbfxd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ikyazvuv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hfhasbjh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ofvvxhur.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cdbtbfbp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uxwpmpdo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ypsmeicb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2deroepbb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2rsserwlo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nnqsiybc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2paorvxlr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2aldingxq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ckqeowqp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jdyrytns.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wgqoyudr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2oiewxcuo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bkswfimi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gbvpcwfj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2obqcfgpc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vpjuiain.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fshpepjc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fegamjpx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uccjknyg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gmtnnlbt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xhcuczgf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2suzuwpow.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qsdpsoot.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2sgggxnpp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2klhzbalk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jhpyqamx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wnbpgkfc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xjuaqyoa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2asilrkxi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgmddewi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdfnnbfa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rdxrygga.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2etgvwfmj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2sfyjmroq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rotwkqkf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmitqbtq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vkekfzcy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2garwdpwv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2oxmcoxpn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vqarqfvu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eqyfxelh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pksoxqzm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blvfdbun.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pqbvkzhs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbhrmjnt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uhvsjzbn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kcfedxtw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ykgpcaph.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wouubdex.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yhdojrid.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oyngcflk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dlmvgniy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jeusehsb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gyzcvhhs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtbequg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vhknbgxk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hwjjxfxk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vegsjmog.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2scdarnca.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nuxmdozs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tvwntrtw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zvkcyryt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vvlmedpo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2blkusuws.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kkgftxlg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fmixjihi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2clejgciy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ksjrdnaz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2grjozrbj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lzlbivkm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xybgmfhb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pkpmdmum.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nfktalzy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ymovzfsl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lymaoivl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2alsutcvq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kbihthcm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fxngnlae.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tlweuvrd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ckdcyter.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ythmudga.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ohbkxyfu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hlrfbjax.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ilupdplr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cstoougj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2sfbhvhac.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjbvvqkg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wjxilrdi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lloolhkp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ujnshgpw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ddyquqvo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uobymozj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofdnsxvy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2flyhfbqe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hnlsjkmj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zorusynx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lluwvmph.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2thddrhcz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xftamlbf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yocfnafh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gxxnlerl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2imocgsbl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2lzaumiyz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2uljmbmnp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fedoihyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhryenmg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fpsckkqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsdvwnyw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2cfngsgtx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jpvkfyam.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmmybsqp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2uzxgunho.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mwyiuqsr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wzhwrimm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dkltgocy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2soxpyfps.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zrefxfzk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fucuywqe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2oyeaxwvd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gxfhgvof.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dovjnuea.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kevttoic.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2plfumbtn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ifkddjqz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zdqzkvsv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2kuxoweyh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tduquzok.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wizqxrnd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2djgqvyjp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dgpkxlkg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wydfkjwu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wgptfpuc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lzcxlkty.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jcmbogem.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rvxhlqkq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2apnezqpb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qgumqlld.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2rizrjvei.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnglgeuh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgbjbfmu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2przgreja.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2uicfyxbh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2clhetemo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dweefhuc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ujllylzx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lpqwuobw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2btiwufoy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hknrnhip.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ibsuneep.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sdfbspbg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qbsodpcv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zfzmnuxd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2useibgsw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xxgkwmcl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2alabavnx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hzyuenbz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2idfkopnt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bpvopvau.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2pysbtndj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vijkqpcr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2enegmkqi.html


<!-- 参考信息 -->