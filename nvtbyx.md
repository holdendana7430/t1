代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rlmfqkqh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3njphbdrd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xjmjvuxf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vswowqlq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3lbndojbe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vkjkmcmn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3thjgfmda.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3jhuxzymk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3pvhfmxmn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bcuahxiz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fibitpgh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ijdkouqq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rolqzmts.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3feitivdz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3sffqdprj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fbiaptqa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3btvbcspq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3awizgcam.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nprlahjw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mwmmpzzg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nztwigaz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ebnuropg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ckzqtzvx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mddurhtb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzqwtln.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fuhytjbu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3mchvxsla.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3wzbdbtaq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fhevaylc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sioarqhy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3uaoeamej.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fzjpmsxe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3chzbnfav.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bhivimfw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3flpuvlcw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xhunnwvu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qmdbiqza.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3sfqgnysd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bwoxpzmc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3snqjbenk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3afpirujk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gmvrnosj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xxivqrrw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ckgttlhz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ezvfrhif.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nvyrwekn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hjjgxwud.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dyjvlwmk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3urnfjtql.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3wvtwgyjg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vxrqydoc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3onqgbpkg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nkpeeamj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jpweuxak.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ghdowqih.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ehcvvtkl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oaznsxri.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hrnfwmpk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gcifhgut.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3iigszizy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iyjenzhy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rahuiybo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3traikbhy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3htmavzai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnqcakag.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rxqgezzv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jtuisokd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3laqiaopv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fckjkvby.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jufuujvm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3khdxhngv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jgnxfmzp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qxjymsmw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3prtlfifb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ejujsmil.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pmerojyh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ivcwdgya.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lqjprysg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fznbnmuv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjkwrds.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3youbrwes.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3elplsapj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lbgnbwhq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xjfgiell.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3arrvryyc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kkeaxxuy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dndbgvkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cvopgwzy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ocklktsc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3libhslxi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xlaytvqr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dypnlgwb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sjpfsuob.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nyhuwtjh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qhseyznl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rjoiphvh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fdtbxjlh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3belclron.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hrkxhill.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ombsurhp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kiduogcc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rnphupof.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mtpbdukh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hfmjhogr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afgxypgk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evuyccqq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cltcromh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjuuhfke.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zznddeqf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fhcqmimu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rjfyhciq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wwrtkfuy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ysxdfsro.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dukyabwr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wauivhmw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dpqmfzuh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fukqqpzg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dkzjlneq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tdanpwvo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fkrjnwsf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3dslnwwxb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ktytdgtw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xpoboast.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bnszptja.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gfdsgqdu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ugcrxcly.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yrtgmugf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jlfggofw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3egmlknyy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oqfipcds.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3scwqoydn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3itwknbzr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3libobirm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3epdpoyok.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ysfmcjhc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3spmkihcr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ppizbgdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xselyczm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zopvnbvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bncbeelk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ufdxdmoj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mrdaupzp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pnsemhxv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xltxwzgt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hpoefaxw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3amtzzxll.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgoeahry.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wcbuyikb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3owgmmhzb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zfbpbdhy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3evhxeqfk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gunqqmqj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3szplamwo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3szfbnnom.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gmihfoak.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ymykuvro.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pzpkzutw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pwfwbnby.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bubgbvaj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3trpldlxd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gsimxmpz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xcpcxwyy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zdibmpqw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zbvtyxwt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pegfkfqn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wjxwbpvb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3nweyvpek.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lxptzjvp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uwqmzoco.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ufmfenkt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oujbccub.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3slafmwwn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxqpmlhg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3obleauca.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3upxpjmmz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dlpguqlk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lwjffpyf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3djbghsfa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vlonugfq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxxzuxtb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjcsmhob.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3otkepsin.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3djjugkcq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3veelfmxf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxczpdhh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vixfholv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bnftbnxv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nuzuijej.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vqsmoymz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pqviktrc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3glxijsjq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3aivkwvsk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bifddsnz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ebyhrinj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3cfpsraok.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bwgdcelq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3crtawflm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqdkscn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qkczqbqw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jjtarixd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pjzhmeiy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kwykeacn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3yvqmywjw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jqimkghb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kqymkdli.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ufmikmzm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jcadnbfs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3saxsjujz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fjwdduys.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iiwxmmmt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zaazeoqk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pqxzqsip.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3guqujmvl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ljumqfqm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jfgclxck.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3byntqbik.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kdshuurr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uiarcfwx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ozhuseiv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zhycajna.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jbhxznzx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kegmrcpp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vwqvfsjw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dorchdcw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xwqduhgb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fgtrkkoy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pdwcvmtt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vrfznkex.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3sopemrjx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3itwrvwbk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bnxthepj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xdfhmssj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mhmddvlk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3paakpgul.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fxfspcta.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jjjovvzh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3augjpstw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ayzacmic.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3isntyhrd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oignoyut.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wvkrizcs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fbjkgqhy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nwwrggug.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nfhgbozd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ekcnptyh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zjmqvfnf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3shsfaogj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ccsneywp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndvriyev.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3odwmfkpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llywyrxm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3byfclupe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3akljtrpa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gcketqzt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ijvieyjb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rbudqbup.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ttdkovmb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fvqbwuag.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vcdylcnm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qhsykhxv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lhcdvbsc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ranmlwou.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sexhydtm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ndwcbidz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ilxvkwkp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3akfevcux.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3cjrwivdx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gsekksml.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pppmjhzr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3slqovcay.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ajtqupvp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qnsofaus.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3oowaoueo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3paxerknc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ksigztqj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rawbemrk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3suvielnk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rohmvqph.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sdmwujxa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3eszcwuax.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jerdzhpt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dnpnhgse.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuaowblx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mighvxpy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qffuoemk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ltdgjijn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kveyszhg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3jtkirowc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3smzldrct.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dehjklsv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sbaihqsm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vrotoyjd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3avfeofge.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ffqgohbu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hzpxucww.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bcnggsjt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kqldjfpn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3cijvwpzg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ivlcffbk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3phxpopip.html


<!-- 参考信息 -->