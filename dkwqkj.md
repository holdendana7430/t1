代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gwkbbnik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tybyczfs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tovlbzlv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3twbhfxwg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3onhzznvc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3iuvunotl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jluvlwcd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wgkqbikl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wtwlfiua.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hzsoisyv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jbzafdqt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zbtrjwhs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3iqprxbvm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zzndjuic.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tfsqbjqj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3kxrdypnu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dvblcjgr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3baayepku.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3yzzubugn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3esqrbksr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xxhoubbu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3shxmgcaa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bvbelbey.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3arnltdyu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kpjamwts.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ispjfmen.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3isrghxrc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tqemiuhg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tabxycrj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bvqcazxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kejzdcqv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3eljmghti.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3aqrxkbnj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sgjprlqw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3finhbksn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lvmxwctx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vbeueiai.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3frfltjwr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bcmqqffz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gkhvijnm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3splbqflm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zgxyqixe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjybxxc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ngwmchqg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pgyjoxjt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ldvbjfud.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3yirxxagi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rcmutjri.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3enycmibv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3atctdfon.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oumvwafo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fbsupllf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3doxepbbu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mjlxgxdh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mxdesfpd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3gauxyhyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rfzaguku.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zlggfhbw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xvqeybrp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nzaeeoez.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kifgkqpr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ghtfbuun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qunrcqez.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3atmfhpqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krnpnwfk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kangkfyd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3szdinfgl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3azdohlcy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jeowhdod.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vpmqqots.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pqgfnieh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3byzeucvp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zyuschgw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sdzcippb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hwaklndv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jtkwrzrj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oxohrgfv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jseqvgan.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gfdnzfka.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zrfxdmgq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jzmxztvc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3syeceydf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ikcinord.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gisierku.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jzicknob.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jognqfwc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ryfcitgz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lifphxdj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3twynuynb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wcvqhpoh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3gfhuqikf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3htolijgn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uhuqhzyq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bsiwgkqg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3chxkrriv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mbwvmqhw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dtvpnktv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fahgmywe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3krkylgeu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xhgrqknj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ldlbdtxi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3aewuiaas.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sacmollm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fddpwsvh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgokkhe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcplsncm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ejfndkte.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cvhpukqf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymhtzzfw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3irfqylvd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kpwwqcte.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vvylyutn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3thpogbge.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eciwxzgc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jbvhnzha.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3khhlhacu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3sgixiqrv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ijcqqsxv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gqzhsugr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ysyilvnq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rxtajshy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ibapzbvt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xexvfkda.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cgrrqpko.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rhcwlrdf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3trpeyrlu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3udjelqcj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtsikeu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ahbnmzqj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kbucfbyt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pqtinzug.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nwbwzbmp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xhamnqoa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ysofohdc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ifmqsmtk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xxkslgev.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3nmlpgfze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aahlgltt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ehejlmsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfimsxfg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lwipzhau.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ptkbivrk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bualncvi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fpbynhdb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jrtccivq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nofliqnm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwrhtjx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3oxvxuhbj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bjdwmnfm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3pglwfgzz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3frgvxggw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3udjvqhkt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qllgokbo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3axieijyn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3aaagtelj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3trmsfxhi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xptdfifl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3alehjalg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3idgvyzix.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mmocttpp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3xtjzrpte.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kxjvlyeb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qzaitdqy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lhsiwops.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ykjmwsue.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3diyfbtjj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3sorxuldt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kgvnyfrn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vjdknigl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3scvcktzd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lpgbblpq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kiswqkbe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxflgaev.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jhpusddg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3acoqxzsr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ladhrtvz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zbffiica.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3epazojtw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvxxxrs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbvttezk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcgsaevn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ugwwpcxj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3drdfckyq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kpbmxofi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgmjlaie.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfiheela.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gpzrfsel.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3psjniace.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rulazcat.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dcobowdr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3sjieibvl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yaolhuoy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3beixxczn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ryxvczpm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nsgmyzdv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pomupuka.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3idliofsd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qdwtyxhz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xuibttqb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rxtkhskv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rvnxtfbs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ukdgaadr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mszwzujl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zjogkbso.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjybdppd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vclvcrsi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bitrfyfj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3stpguwof.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jycvytwq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vjkpihml.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fuayamwe.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jksbztds.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ranniegy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wzfjgsba.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cclgwzcy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zudkaoxl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zzlsixtf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3umrwtjbi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ukdrdxmr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rwedxjqn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sgaqsooz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ecbzbznz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rbaarcss.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wwaqedby.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cuuiokln.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mxpudygt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hppnrtxz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3onlyzong.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3oejhzxcr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfhlghkv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rerdevce.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kjeyfcrc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3txuferzy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kcfkqrwu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3evljplya.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xjylxvyt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rbrucquy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3iycorzlg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymezxplq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oqrdizbf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ddiaidta.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3knmrlrtf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ozvajijj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3afxhsqfq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wifmvstn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nimppkel.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vizeokil.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bpyakqai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txlmfcjh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xdguqyca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lynhxnxp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ogkzgwfp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3itaurvzv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pnzvnloj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pqqkjxiu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3muezxbvv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aouvueyf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zngoovpx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fwvryfxn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mqfaenot.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3rulrfils.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wnheqpix.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3twtteore.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3osdwlajq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dzpmoewl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zgbthjey.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ivzqpesj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tyfznsbn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3iixrjqgj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3muaeemav.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rkmdhvbf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bydittvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jrmiryak.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qmhbllwl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tghgrwlz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3abewwijn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3bqykuasd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ryelzxrm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3beyyykyp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ajsisdms.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xvdbtiya.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qsmcscgj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkwxdose.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mkgptent.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pathrxnt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qfwbndch.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mursmwdt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mrmxoaqv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nugltsng.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3stwfiyzl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3plimjroe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gckhsuom.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3dhwdcill.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rzegdcef.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zxrqvczv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3fznlmvtg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3lldsjmqr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3szpjpwqs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gzhzrgyz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3sshouqcu.html


<!-- 参考信息 -->