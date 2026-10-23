代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bovoosfz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3sacahwpu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ygvjmyln.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3grkjxuby.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zmsthbvn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pewinbbt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3tujnkais.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3osplxchj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qcdmziie.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3epfiaasd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3luywvabl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ihfubfye.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3lidpocvy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3byojnttb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xqdmbwan.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3arnqggjn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wrnowheh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3uovjeyit.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3uylgcoix.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qffnzsfb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hzdiqtxy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gnvdcaae.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mbyyehii.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ukohzybs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tccrbmpg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3sfvtzsoy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ngnnrtwy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3udquqlvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tpaiiace.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qdvdvbuf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jkrrkyrd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3dgulhwai.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3hkehoeyu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hzowellz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qmnchfzw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kgzeaxyc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vgiceccq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3sypdakap.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kkcduome.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vrmuhxqm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3asasgiaq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nzsncydx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jbpdtyrw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gfxuvuaq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fsrjhzov.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uvowfgoq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3muxpaasr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hilhtyli.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qgcnhekb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ltrmxqxu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tcuwclci.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3maapuydk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bakcjrkv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3eqswkuql.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vtzzpgtd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kohtxoyn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3njvaqwse.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rkskosan.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zrmzjshp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ieubqnod.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvfimla.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mibsgflp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjasxjrx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xhetyfrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbhcqxqu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jphkjfvh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vqwxrfov.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ufoxwhti.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zojnhhtk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gvngykon.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pmjopnxc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ddyjouus.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3onfhfpdo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hezwkmwd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xkmycpnu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ogophnhp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zmqcglfv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qiynnqeo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ragjgucz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wnyoorvs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3imcltjxx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pxoapgqf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tvjdhosh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3pfsmqwku.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vjjqnumx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3uhktciqp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3trrxnvyy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dubfjcdq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ggzjitus.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ixndwchg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mfqufeeg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ibmdsvyl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3eyasbghc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3quwoebek.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lytguhwy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mphayaqr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oshgwpmm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mqcsfhvb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hflqzcyy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qpzvonzw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3efcxksyj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cuotucjo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ccilrayl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ordnswvj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nmuledta.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgbwzqyc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wehkffqq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kyjrgofy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fcltbldp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nuumwxyo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3onyiopiv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xbwmslvv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dmsgvkul.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hpkkhriu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tyoaybhe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vcqjczmr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rxsnqbps.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3yclxsgao.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3racwkjmz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hctitzpg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uxkpxqaz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bopisqxx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wsoxibcj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ancnxahg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnrjtpf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gktdxijn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tvrmxfsu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hbcyuewm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jvwurqgb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ialeygnr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nkfxorqc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ndptbjhz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bhgmwxlx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rzslygdl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3llcqhfkh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mwuhpnlk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3myhnuvbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnwtlscp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wpdarawh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkcspzsq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iycsnxsd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulsvmgji.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dapnehfd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qsgkebjt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iodxeuqp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhpjqxzy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpbgfle.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jqtjqccl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xpeqcbsz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ldmtvnvf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3aeicgwfy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wdxtnrgl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yhtdbfpu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pakukgkn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ptfixpkh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3muqzqlfz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vzkefeab.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gmlruhhz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yqooaguo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tbuybven.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rgganzpv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vbigrnak.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3inebyqfz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dljcpggz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3msyiesca.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nhvzcesz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dmkgmtad.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sjmnefvy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xyndxgag.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ajuhfcyq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tkfrxwwe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qhguuvpd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksjqpbor.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3tcwcnzje.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kjezubji.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rxlhbznj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xxyugpbu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3badldgxx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnsfzr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhtcvhqj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yacucglq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ptvqzyrb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hhohdwkp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uzwdejdz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyalknon.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzolecrp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tukcvtxy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vsmochys.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3axlyfidy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bcovqyvy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3danxgpty.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3taxmbrtf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3upqgzeuj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fsjnesdx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tcvmthgy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3gvbaynsh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xiqnabbm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3auowkyiz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hdifunuw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wpcduwmi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gxoloiht.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hpcxjnpb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ccuapozr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mwhakaly.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3czxlrigi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ocyfkyio.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3acwhrmio.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3acequxsz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fpuapuqj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jceaohmp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rgjvhqmb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3noauhnek.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gaabxfbc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fioogphc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zzrxhxbi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pfbqznxx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kpizgkpb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zpwgvxda.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3phxnsxzn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ahgbyfht.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3tuszkari.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3onslailo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ncxysvfa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgffvszx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3clpruysa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ipmvxkma.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3aygozotc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qjnjugon.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3aseldtkw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3alufgkeo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hwybngaj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3cmrrqsxt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3caoprojn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ntovzagn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eayxtmtr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jtluqjck.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zmktiips.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3flalkhvh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vvedbifb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3awsncjjj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gslqsilf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3sxyanndm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cydlnaky.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jjwoqupt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gtgmkcza.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jcntvoqf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mblbembi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xznmoqzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ongnrofg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zphfahzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joequiib.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3inntotib.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3snhivynp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vevfkevw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pysxxehz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cnnhmopg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cidtsmqf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yhrfaipa.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zexnfcox.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3skttfxpp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vahxcacv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cvkwtqjl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jotxkisg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fekwgjzx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3petkskrj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cdxryiuo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fdwrhkup.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zkoeotwx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wnuxzseb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3upujcnkj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ywwpzhwb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3blxtlyks.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3hkhiyywj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xruzfqaz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhruihnk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xtbuqofp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bpzefodz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymmxzczl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ootbooeo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3krymarde.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ukitgedo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3obgcnynw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gysbzfhh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yyuzjvlh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3snuusxdq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jpparvpx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pewbqcho.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hydvzecd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ykarsqtd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3oswfhccw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ymxygiee.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjksvnq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vdiokgtm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3oioorifo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cjmnipvz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3fsvweptc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3rtinuwwp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ntecwmjr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vqcfutia.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rjfqbaiw.html


<!-- 参考信息 -->