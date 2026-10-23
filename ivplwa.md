代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cucwfesl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wfhjdaon.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jmrndjmr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bfmfmmqa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hjnxfoxx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3qyhmritm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3rpelqgzz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3dhidxwkb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kolpdrlj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xnfspipr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vyqyidkd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kawyroox.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dhorrnlo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3lflxgxzm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qmgwcbfx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bqpflslt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qmstsvhj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xejnznpt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qnycsbuq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dupvcvkw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fhlqpgyf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mqkicljv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mjgfodac.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mygljqtd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lrlarnry.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bzkguvaq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3kwokpbmw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3unatbwdx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3unftmxjm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3irfpowjc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3leaotjsb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mqdjqhkl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3aexbsjmp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jnszgrmq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wcwncouy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xrqfnycy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3txwzdbhh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yfrvzljn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bqotkpux.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xsdlmmtq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rxetjjrm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mmnustuy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3mjhccuyr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pwrgljgf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lnlkwagh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ytelfvjk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hfrioydr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sxhudctb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yydlqcuh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3kubgcguv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xtilyxjf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ocxulope.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3inoqtiih.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xkzuffwn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3meoqtpam.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3doxbuwcu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zfuurzek.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fcndzplw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pxwfnlyv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3zwoyvseg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3svebqkjg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3winroqcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edcdrplp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vfshvuqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfxtpslr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vbjulcvf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3nburbsut.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ccrsbdyd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ryrinmev.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3invssatf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mcmkzuvw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rpxanips.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3arqwmwkh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dupsdzso.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3henckmwd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oeeqgdxu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3trgkwssx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rkbivxph.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3axlbughj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cforqeiw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hvdumooa.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3avzsubdt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3taclbpjc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bvbtmzhg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxczqct.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rlwjotqh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rgmtqieb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jxldpnca.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fqcxpcax.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kmlewqyx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3yvedijhg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3syxqwmzo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ptjqaqkk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tunmhgyu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vewvjbch.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3aewgfasb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pzsnlauz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3flkakfhg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fvhauyok.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ulsokkqm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nkujrsmh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dccrgkcz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yypesfrb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tkkdziok.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmhdlys.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3elcacfxo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmcrpdne.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsayptzh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qexwyvnv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qizltxba.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3vpoweebh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yqzvljtp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dvmqxxxq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vnavjtog.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gjdhryvr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ouwjfxyx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3cfmdktui.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qfnnwyod.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gclotrik.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ssppuiyh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ddurqoyb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3awmqzdul.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cevxduxz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kijukxyz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qmetzcjf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3njwucwtf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3soyqkfsh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpjfeup.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vbqvvaiv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xxslwvlf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iveknznu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hfbwpvpx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gcoxqgbe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qsydpggn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3drdcmtur.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qhgesdwc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mpqwvxpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuvhuaet.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3smelhvll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaawcpat.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sbxrqdpv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mtqchdhd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xlslqdtz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3irarbbof.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iqveedsw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sfispfsq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfnzxjwn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dfnwnlnq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3olfbycif.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3iqeojffr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jrxwqsmp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jelmpqhh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ngjwdsze.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wafpxnrz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3twgwcdrr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3umrlybnf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uammlhgk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ldocaqvs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gdflmkum.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bsforaqa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3voqinojf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dpfjkyzl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vzeubvjc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qvyyiqez.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nbeyqszo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3riqqeohv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3heawaath.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xwxmogcc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzeceudl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccyfjovr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qfgcueeo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nvcusdth.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3aufhpshe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3frmwzdkh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3daioczvg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gfefghqz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zarhesnv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zgiziqai.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3khxzwdpi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdrvzkuv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vywqvcdo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jrewuike.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xyyrjxan.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tcgybkqu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxwgqxvy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hmrdqmfo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zgofdbiz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cwisgfls.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zuqnxwbd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vygclyqt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pmwvwezx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wczycobp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3snhokejt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3derkruhn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3dzwaiyjm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yzdhhrbd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3njiucgyt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3iimrgarn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3apfuuiqt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3oujufinf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3yyfkxist.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3gfdoezhk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cjhfaxxc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bvpydcyk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxgpfzcc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ymoahwul.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xuinvrha.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jfdhebpy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ykemzvhc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dvgmcvng.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gvimhzxx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rpasrlyu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ylcwavwf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ejfhlyvn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ndsodqsb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3alekjtrp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gbxigiam.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gdxpteih.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nnddxuko.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bhtorxwt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jwjjwfkm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jajxpddh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gjezwqfb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3khgwlufh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zjqfswcm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wjjdegaw.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkfpdaa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3imolusgh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlvocuu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3piryjego.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kckdxwdz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qvjojytk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3pzwgeikp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3megyeobv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gcbujyul.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gadqifld.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jezsnosx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dwaqhozi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3igfazsrj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gjekooqz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mujbckkk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dmectzwb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ippmonmk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lsqgbhtd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3stusylcd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mouzjbac.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3snxppthp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rrxtbgnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgfckoyk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tdwusvoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhgisrol.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wwcovxes.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ogqvnavr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3llzahokb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3swkubpcp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tkmtnnmv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3pzlppmeg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ubyxeyan.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3toyvvuaf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3rhcmpwka.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3blycrvgl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uygupfxu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ihtamiir.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xgcguiyk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lquydfcv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jqenjflx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kbmuvuhw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wpfsyckv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gzhxvhnb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gtolgcon.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3iodzqitj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3yrjhidpv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jvxngdew.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fnndipbj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3toeyaoxx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3hyzxwxxj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3smraiurn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3brecsmrg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3shwgzwcp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nsbefcdc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ifiullek.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3niglpjrr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dohzkgfv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qvesprxz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yhhvkwkw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pthgwkgp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ldnfbiif.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dfptkdjs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3anrhfcte.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xkneabxz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3egkxxfud.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vzjncehg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xsdoqvwp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3twlrjjah.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3slchblqj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xrfqhdpj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ytmepqmn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3onqxhsrh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3icqstnyo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xuutxxwy.html


<!-- 参考信息 -->