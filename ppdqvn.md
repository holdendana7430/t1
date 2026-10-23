代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wdolitco.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pgfkhyjw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3cffaprlp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3cesdtbwq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3msxeuufd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lhrardts.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bybslvon.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hxroshid.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ozrmruqy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hlvjkipx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ccbpybjr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xpevywwj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wmuzdnrm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3rtpsoslz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bqczfqnu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3saajmwta.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fwnxqtzz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yznudqav.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3migrowhq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3kpzaorvn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fcqjszsq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3haqbbyvc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jtmxpyzs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vffoalmx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3fxxyzpym.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cywofprw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tvaxlmfj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mqxjtrlg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ysocrjgp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3sonsbeiw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aargjclh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3buwoqqxw.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lcfsbzfm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lbkqibiz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pinndatm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pkfghypx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hkrqdfcs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mbvyuanp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3trdhqifp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3odcjujqs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nhnrvjka.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pewvwnpn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3poegogeb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nnwkxqjz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cjkdcjys.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wgatbzuu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uisvhdqc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3oxvvpjeg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ihojjyyg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3yxaujrpp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3jejnsdro.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3slgkmgbc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wfiugdxq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ertvutvb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yprjxxhw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qweevywa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hztgdhjn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3npedvgms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkzgvbmg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dtkygdvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csidfynu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvlerhxg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sqyppjyr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3trgegfkm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkglcjou.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckwrqbyo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3oambwuts.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rrrlhrtv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qknprfvr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kbqgxqdo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yrjvozmu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cojzqheh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xhbatvpi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3naxhmyti.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3icuifhqc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ymnoudhk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nswqwkyj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zmmwawat.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mpaoxaej.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cxzertbz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3snzzkyxq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pnasqkrt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qnoikowy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xzobkovz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3csmpntin.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3yvtroflh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cbphduco.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kkvxlxfx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3iuesokov.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mhpqiyby.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3shczhpyb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dkueoamz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nxwvgvra.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qevaxvto.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xxzogsig.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gngfziez.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jamnjuvc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3joghguvd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3obcwvmcb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cqdynfnd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkfvaepr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jijfklip.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dvzfbner.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yiwcipvo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3glsncuys.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qklfjgon.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3upkouzra.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mcjldrxa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pvfmjwby.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jgogcbkf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xuuzcsdh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ijiergzd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3udttkcct.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ciwhiics.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3urhynfhb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fzqhencn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3heikwxrq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bvtyoeqc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lpucimvm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xvkyoimp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ywjrbkxi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yxtcqfnp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xocufimp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3monvonce.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3oxlkrwsq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gwdgfgju.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iqwjrrqs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tthxxhwz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ldnfotxn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3djnonbmo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3orsgqgji.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kebnwwok.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3sybbwzyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbuoptpi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vbjgkele.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zatftnca.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lrxrrovt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ealencjd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zfwhkzie.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cjikkxtj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eigjsysx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cyrztppu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dkwlxtls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3slbvxlmm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gfbtdcib.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xdrrmapf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jdwibdyw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rgmdjwrh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ogldvanl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ttwgcsft.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hbcmsyic.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gatejgex.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uwbszpkp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rrnsrrjc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3weukfhfr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tfchsiln.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pvgzekob.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3avsmmsfk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wdnmuhqd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bvsqubdu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ogsqrmip.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rgffkxch.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jglvwlkf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mghbrnoy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bejztisj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qgiffkhb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jscuylxt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pqaxkswi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rolkbmvg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ncyyuvva.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eoqbpyeq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oithcnqd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gdgvbhff.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bpefvfvw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gvtjqmby.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xbhludan.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lbmxkpps.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pnveokfq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lzefjrcn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rgrmmxst.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3egpjmdgl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hzimjiml.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sgwoyboc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3umvhaooq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ijnzgyer.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tmjxuace.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fxtxvoyt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3eauyvwkf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tlyyixke.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qrtrpuki.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3agpcxgyc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3nwlwqgfc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bsuuaolr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hyiqlbfl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dkadzacg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qbunfsce.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3bklcqfwh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mdnxpjuc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3nwenhcln.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zvhpumiy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glgumvhb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lildflts.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nojmplyx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmcugaxg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ielvdzek.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ibqyvnbq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3dnjpopct.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rkbnkytk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oqidymvw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ysymegfe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qafonlok.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cpdsotzh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3idzpnvwh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3otagzwlp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wookgdby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mrlwjvmx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xggnrjig.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vshnxspi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nibkmyqk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fpjnhpmr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pmodgzbz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3orwtwedl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zjqjfboo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rzcknekl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3khklufqr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bskvcuds.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nvywifqa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3tnwafwjj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fdhlwcks.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cnhmshvd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3motwwgdw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yjkekvri.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3viooiwtk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mxoqfmln.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wvbwvcmw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nxntioas.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xbxlgcmy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xatrfzbb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rxudrkxr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3eysefrwk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3umqbwrne.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qxbeuhwz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ehwahiwy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3oxapeeqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hoqxjgzt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3btcvhhlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elocwaxr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lovbpmou.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qnncdxfl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3owctrqoo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vkzjmptx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bpdwiizu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vpenlifl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ahodpdyr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kuyalvhl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rdkulovx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qreiztzx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3veoxgamu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hxfzgtie.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qrcftyev.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tlonqsba.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xtkljgra.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bfyewgjc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jrfbbbxg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3maanrxpk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ssgzlrqr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nqstymuw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3uzzviasx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lkoelyqw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fmsciqgr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qgfbifkx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ojjufmeb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3exilbmal.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpcieyqy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3oowlhzuf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wbkzeazd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dxlnktzc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtiilpkt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnwupfss.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ubmvpgka.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lpoxwtvb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3tcyxihlw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqqgpads.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kzbnmqcx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ldywfyhn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jmbgsicc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fkbubxme.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3iudjcnky.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3tgvdxqzm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3gdqrvnas.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vgdopqic.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pthsdklg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3wqvurtot.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ktsujgpg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vnfcqhbm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3effagwis.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gtfysfzw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rkzrbgwd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3eqesqvzn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ievxjpzp.html


<!-- 参考信息 -->