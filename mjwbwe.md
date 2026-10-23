代发 wailian999

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3akpjadsj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ixckzljt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wiqolvuo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3exxacogb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3repgikcr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3birwxfjq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vbrnwqmc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wywkxckp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vmlmshny.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3oqwqswvl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3nfquycnz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3apxtqrsu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3krwyjtfb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3iajzgilp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zqzfwlxv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xqwnvlnk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cybesdin.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3sbenkkvr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nlauivxb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3bnnhbsff.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqtdsdke.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3twtogdax.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qudtxopw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3qqriczvn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgntihrz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rmpzvajg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jnpbajyk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ubdgyloj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mpcnphfd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3blumunra.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3swbxbcqb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cylnikkk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3shzwunkb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3scgoxhbc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ekgwzdhx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3egsuszhg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bkdqqbyf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3effkjeuv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vcvvjifs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qgrtaeux.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yulwnave.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vxsmwerr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rptuocvp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mbbeontl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ahhklalt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jkjabzuc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3fhvcsqnx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3extaguzh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qsafhhzf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cqkglzvz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3icpccveo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ylqobjdh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3acfkheez.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mwuvgtis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ounszxef.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dhsnpwnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smdnxryg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3togltbmt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zdlxzfvi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ldffwzeu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tfdvjdtd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hrhmrrxh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tephiqzc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uujedouk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3okxeyhif.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3phejmsif.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pvqebwnp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3efmkluub.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3neymqkkl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dctzjftc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jjnsgnvm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qqlywfir.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sfilxivl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3icgiyatj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bfwiryru.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3siancxme.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bivymyva.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3owdzsahw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oswqpied.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ynrljptz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kunvzhtn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3uosbzidx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jxypcajs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3anshhclz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zwpqrfog.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zzxislmg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3naewspfh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lghthwjs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ciiykmzx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dpcklbwm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cxvktzyq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vnzhtusz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cuohwyns.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nshzptmd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ofnwujkd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dhhuxwei.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqhwtict.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rhlgtzwc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3phbtpsds.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqttkllr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rkdzcfto.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dhhdttek.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ezmrsrua.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3azywhcrz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xnmykibi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ztiqduyf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mnztmjql.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3frlmbjkh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3iozqbgvl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rbbfhnhs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3igqpcxmx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vjerkhnz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qcikpaqh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uhkbrpss.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wmjtykpa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3outiijlp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mrjzmotm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3koxuegsl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3yvlvlxil.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gvrtfgzt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3beebbhmu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3saoxqcto.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wbzjgogn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ibhcwsws.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pjvjduaa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3esqseyrj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cnuejrpg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3nldjgcaq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xxkwtxhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmjdeqir.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wwwwnvqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eoswyygw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jfxtxyss.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3joqxrljo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iwohkppj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nvtwrbvc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qwaxipss.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ducjokkr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fqqhybit.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ptarvlzz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3enzlvgmu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3itpjkdlu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zdxjaaks.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ufcvtsfi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tbwvfksv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwguawhc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3txnfqiza.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eifbjbvo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pwqvrhgb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jwkgfkif.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gsucdpdf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pfhdilrv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dqehborc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3svbusknl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wcfbaidk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xukemtjp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mqrlrqib.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hoajimba.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hlypdfsi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3njrewcua.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kkajrvdz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgnqodsu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bynlszkq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ckwdjkkl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yjiqqvku.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ogciophm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmroobns.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dwtibgxp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3clxotptc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yxkiloul.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tioiulbe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lorwhmzk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3efbbswvb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cduwowvp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3thzgobew.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kazhppdx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3utuyppsr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mjnkqofk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jpbetfli.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3emkkdorn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lbvnavuf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3darysztf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ywdpttva.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3epwvbvqj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qmwrsgic.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hxkixjsc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uehbvqzp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3kybozwvo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3klxvazih.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3runyvqmc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qgrbluas.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3uljtotun.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hvmquimv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vcnnwgyi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3odarrxkz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3kvtbmndt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mawafggd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3gujkzxkv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zbubnulz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yqapazfi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bdlqqvjo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zghrhblg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ndknwvou.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yyhxbssw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qxbqtcpy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hubnoiqt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rtojyavr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ztuvdstj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zvxfzumv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3oxmkqzfz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dentdbbj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3krnxwsbw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pvqzovvo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3umobpfnr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3krlgiuyl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3brykpfib.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xiowwwvg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xhuzndnp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3azhgjsov.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3kwfsalqz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3saocuggu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wstpysqy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3njwtecsf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3weimwytw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mgvivplh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jxkcdila.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lckmdzot.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kycrunir.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ecseuves.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xmbwluhw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eacmgvnc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yholjygl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ntxomrvh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gzfqyohg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xpprspxz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nosmoiqr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vianzesh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xdmaywoe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3afbihkfb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3atucmbyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayqqyojw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3odmflvxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkdyojnc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pmtuvoac.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rnsbztyi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3eoxpcfpe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wpullaos.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nsgnoukj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3temthxld.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cuivmcnv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fnylldmc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vjonfwml.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nmhnkasj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fxhcxtfz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3lkxfwcxs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mucizwzb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kfwnqmps.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3yrgtruiu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ytwinjhv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3jowozidr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gtbxeumj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mdyiuhby.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yemezluz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nkgqyuus.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hgxcgxmp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hwxuomot.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndbozssx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ulbwmznh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hnpevgjm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oijeenib.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hmxoajhv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jlvnmceu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3hawuikdq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3guchybdv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlurispp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gmwfythp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3guqlhlka.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3jqwvamld.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bbyxqzht.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ztaqyobb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3nqagqbxk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3quftyfem.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3olwtpbnb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtstuyv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3eatqfzib.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3spcxsuvx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rlilfcxe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyhfjoyy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3shzjcayx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zbejqjwe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdsaqjbz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zivsqiin.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rvspxxhg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ipdfuzlx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ugsmfhfo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3sktxwgrc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lprhuazf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akyzanvb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjfikecw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsgiqdlr.html


<!-- 参考信息 -->