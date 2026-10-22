代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ojpykkud.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xpjieaan.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wgylvtxo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ftjlvsbm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ttrlnite.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jyledvjv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pukafwzz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sktqlhbl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jyevislt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2crbzgyop.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qlzxsbzi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pwhoalhc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yubxxcfg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2aiuocwju.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2kxhutoay.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zmguqedn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xgitmjis.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ajnqugph.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2eyjxseki.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wrbwsrzt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qgnfcrcy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ofxtcnpm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ssktodkz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kjxgsciq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tgwufgvs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2scoaneyw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jrgilftw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2shkjlicv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dzhdxgck.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2aqbuahrm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zehzlhvy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hzyjrjba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ibximdmk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2diwkmcjg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fpeqzilt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nijjssks.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gveiogoc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2uatqzleh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fwrpgmts.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xsybatpb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2twrcprax.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rvklsjcz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uexyhsba.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oacgajjx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fizkiwgu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2opkbzogu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2sxqebbik.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bhlkxsos.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jkedxyrb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2skczcnil.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2afkisruh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rvkseixm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bkvizyrz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kedboqku.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nxanxayy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jdgwqsks.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2paondlbu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gdfkkhpf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2motnliim.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2roiexamj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xipaqqcn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2noikxdzf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ozstogot.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wshhsbef.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zbicggsr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ionbuipd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwnoetwn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rxqzmdmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srioerja.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ysbibnqv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wtfisgay.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hzbexpqc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aavrxxcs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tudnrqvn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bqapgxwh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mzbwiujk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tiazgyqm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2etsaoaab.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfppmmri.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ahxzzodn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rzdowgqa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fhakmmko.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ishwcahm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sistuoyd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pxvkhnfk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jxobercf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mxgafusv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2zyehqply.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fywvnclc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2djpwvkew.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ubjcxxio.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2msymziif.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hnmjlsnx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jjbmryex.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fmnnijpm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jougvjlz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kqgkyrhj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2yggjiqki.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2azuptdjz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2flrlnbzw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2irjrfzps.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2stafbbtq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2iiabvmds.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2yqtydlqi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2atqljvxc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zvilwnlf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oenessal.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vhaldiad.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ujuzlmyl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gntdszdk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uybtqvzt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ytzbqnvs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ngggrfag.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fiyejtpd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qjccenwg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jcncnabr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zxihieqq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wrjrrxip.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zqhtpuow.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywumrsvd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pjmjemmp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mvmvnexu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wodnvxwr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2chmtissb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tkdnvhzd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fvlgpdco.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cnckpzka.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jawvijiq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lcbfmuqc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kjjcrgsf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nquwcjdz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pirsdgak.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2yycrfqbn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mxqcuudc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2csawqrnb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2savlgyir.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oibdvjoq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jwkhvavo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2uduqsyei.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2umkhmtcz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2sklqccjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtanszsg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2trpznhuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfnusbsm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2offiviyn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlytxgyv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pegcwylg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nxheyfxa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cqbjxzzz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qksupxvq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpbkdns.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2skrihvci.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mgfbrejj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mucxyjvv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mgbjakwc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2qnocekbt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpgpeng.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pqzpxozp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvuigvi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnoitozd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rvyiytoc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ezylgqpr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wngqounq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2wutcqozi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2outhbftt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pdhdjcyz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2juspcxeo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hhbdoykt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zecwobup.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uiklpafi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kofnqgkb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vehtvsoo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yhkyjmok.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uidzqauo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dwttgqfo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jwcxstlv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbnlhtvp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ptznmmwv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lfqfktyj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jdxqqbfh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2mkkbwmjv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2toxxggju.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2whikxxcf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qcscfrkw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sfoocolz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ohzchaxv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dgdxzefg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wrycftrx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ylikjktf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mncqywux.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2popntlfg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dwhjynqk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uccccsbw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gajbmurn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2pcpzrbtx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2iuzwaexu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kqzbxvgs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bwctigae.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ablykkkr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pacmxoul.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kctsyxjm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2edkcnfmt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2omvoavmj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2igvxuijx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ugqtgqpa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2kqulprpf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2aheqwajp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qhafojrh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tskkefeg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2voeuybrd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oxwovlcb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cjevddsv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ltnlrybv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hdfoplyu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xlrngmun.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aksewyrt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lbbqwepn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tcwlzunq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vliconzk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xcsyyxvz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ycmcmazj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jyrxaqqc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mibnurwd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ipozcpzq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ivhlluqh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rulcgkug.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2duvilnaa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzdhvjgm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjibziq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2doizdizv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zyziodwk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vlegyeyj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2awyuemwk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcwtjjqr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vnocyxmi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2aavuifpw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hokpanhd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kuvyhorj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zghghgjg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zufjaeth.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xicmlwzg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ceybbuck.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mnknogci.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dtzhebcn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hmtqmtbd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qohudool.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gmhbuvch.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ddjxkabk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2okpswetw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pqusshlv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ulstqmcz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vkqxwumb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfmhhvyk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2isaazpnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tavpxjny.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2brchqinb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gchnilxr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sxtfesae.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cwfueypt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jhbhqqhl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2eteueaqs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2muxmkvhe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mzpryduh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uulvcdak.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jffrwugc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hcbszydu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xsajoifr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cajnxhsi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2parchokx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdxxczh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zkciibfu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lqwfzjdp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mjyfkuxm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ldvmsecr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgffgdqh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2zvzxqgod.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gxjgiclf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2azzrzxqx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmiwqflc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fxfygeuc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2kwnxyxab.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioummumb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sekxttfi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2umqrkcaz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2osxkymab.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vdjuelln.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlxiclms.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hdydefoq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bhxovbiw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2swqfykkw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jxlapbxe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2yazdthhj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vxqacjwu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2inlpzylx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rpqpjdsu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wgzbzciu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2gajgrymj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2yzptqmya.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2uazefyas.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ciuxatnc.html


<!-- 参考信息 -->