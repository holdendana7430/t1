代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ijkynlpd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ipphpipk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pchsxiza.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uxyxymug.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jtlzmfyx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2crunrpfv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2nbkwmocx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccvhlzuo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ftezhylh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wbnxlomg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tdtjtjml.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tbdskbas.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rtjaczof.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2icbzaqvf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kxizruej.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mwaxtkws.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ismfuofc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sleoqaqt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2medydejf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hgfnjwuj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2oncttqfn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uafqqpsp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2urkhvwry.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rsbuxgkr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jermqjhm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yobvdrgb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lyvkmfrw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tfbbugrh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ekmvvkfy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ylxassws.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vdykxorl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ahoezwlj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2uwehouzb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2slloshma.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tlvxyphn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xrnpsuia.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ovmpvvly.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oceflmiv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kawklfbj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pzjesrfx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bteszfgm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hbdiuwjh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2punuayah.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kxffquhu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xfopeszy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2oxtatmcl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2maqfylga.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nfbmpyif.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rlzocfct.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2oboeksbu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zwgsuslt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qivwqnfe.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gqypyzag.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cjlrnsab.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hatregsa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ksxcggno.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zftzhahy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2erdiksnu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2slliewgy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fxyliahu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tymsqdow.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2eegalvbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmjndvrj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2bbqhohoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2notocfhv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vhryyjnn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cjxpyiwo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2yfexyeku.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sxtvhhjh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xhhigneq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2utenjwiq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2qxqnxmvu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2kdfpotdc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ogsxmxse.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dyahxcuc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mxxshila.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nvxldzlj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qnctvxck.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pmeheita.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dvbuhhbt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2julopasd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bumzpbah.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2svvkjlay.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2plizutft.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nnfohgtv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2bkwalqxu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oauvgcga.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cpfqassf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mxesqwpp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2oqvwybea.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rtqyfwla.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2luiqeltp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cavibooc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gnipfeuw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qlovlmgz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wlgxwozj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cshaunfn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2yobotoeo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ijwvjflj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dvyjfjtn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xjfjrfdc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2iktinofs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rthtmtkf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fqpzycfp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uekhibyf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnrrffup.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2olcfrnry.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wdnpsuvh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2snodufpf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hhlfpgas.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ulkdqzeb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmkeipi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2btnftaag.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2trvfkrub.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fwmtwvia.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ydjajsow.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xgjlfmsu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xzykomtz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vsflvkjo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cflnicqb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2afcoxvgy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2aurbeyju.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wcztqrhm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vwzpkjyp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hmzmuqge.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kdpjyqgw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rrwabovz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2nlvwfmde.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fonihdcq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xjeqbofs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2agttnwrr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2menljybn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2iknpndfd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vwscjszf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ronaehqh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tdhfdljy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rxyvgzsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqxokoek.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lbdjcndv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twsrvsrp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2huluruzy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmxknnhu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ktarjzwd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gcneabjz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jaiquaas.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jnnckutk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vcfebmwj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gwimljyu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhntocxz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hswojnqs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2juawcfqc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2udxiilse.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hcntybqr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tiemqsom.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dfbwikjk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yewkgxjr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hxiavyew.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2odseslnd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wqilxtrx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kqrkibhe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vpijvtrl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2iazkkeao.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dugafjcj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yuevtfzl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wiovgmua.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2behdjnul.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vcyftcik.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dmtlaeme.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bprsqvps.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuomlxqi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vdluynsj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xofeggla.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcbojmvo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dnrgdzuc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdvsjvg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2liysuode.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qxfvkrie.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rcmkbqdp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cpdbvlcf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2objlgfoj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2abjddiig.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2pixidcbw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zojhxmxk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2djdofwqj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2eilrjsto.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zueppvpy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wyefklvp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isklxzfc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zrpahlco.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rlbpvlsb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rsntvaqz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2icfnvxlf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2afyjpgmc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bekttvtg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zfmjganu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zfpfzucl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2iqurkvdj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mncrxtmg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qsuiqfya.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lbigtmzz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dwmqofut.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2kifhorfm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2blvylqlh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fhyvxrxl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wixmzdiz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ecummlnt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vcdadjjl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bqcpemlu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bjushvnk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gobnoleu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iwzodtuw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iruiwiyd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qgyapabl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2narqlexe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xcmnqmmv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2afympxsc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hldutxzw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fvllacnz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bimxahad.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kftsjodx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lfpmflkm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2giuselqu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vaxjiduq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rpdbjpiv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2bhpgzcgn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qrgyfvbj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2davqrgdf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2uinengkv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ftlzdrvb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2skrdkcuf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xlnsgwyk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gmqluhog.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yeyedtqy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2llkezvgw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iyvpamnc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gnjjohke.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2smsyunfi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2sarlhmll.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tqulypuv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2aiieuqat.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2iznzvdon.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yaevthts.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mandocyb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ecjriios.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mkbagvgt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2czifutgi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xcbqigxf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cyqwsbeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saszcprg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kcexoxsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nvgseqxu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2cffdoqbu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jcgsznav.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2biriiqik.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2eydqngya.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kuxnzdbg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nkzwihmf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zprhovrf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vhvdvkkp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2oucgijtc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2crrgkmwh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhpwznb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2coouincw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gkfnovfh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rmvcxcnz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2exdpbvhi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2azaetvwk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2iggsavxx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2faixndld.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2aimaehij.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xdgstvyz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rewbcibk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2flwirdrm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xjddtzuk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xobwufcz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vgxgyrvl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jrrqzthn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2axeovdrp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yextifdt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jugksglq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vkrlgurm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hhjqfnuz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lonepqya.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2osafoqar.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2eyhotowh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ormdritu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjdbkimn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mlhewsmg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bbyqbrsb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tklkiqvy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2okyvcnqe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2amjvcozt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2earsjtep.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vvabganb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwlikdw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2logutgeb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2otnstica.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mamzdqqu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2whccnjkw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gemvpnbo.html


<!-- 参考信息 -->