代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3uidiuibr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3coothvpf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ioufnbmd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3iqtynvge.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ktkoxvke.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3mvetebzj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3eftorfqo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vglyidvg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3duukmecm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3texyaglz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3wequbfrc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pfreqmcl.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gxewzmvp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bysalqhu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fonbbmjv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ztzhcrah.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ndbyobgf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3upvodmit.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cdkpizea.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3eaeskiyg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3revyaewg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bnneprmb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bdxlzsta.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3orssvoyu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3iserjuad.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nqsbchzq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wlhvjent.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jqphpfjy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3eozymsfp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tlusbkwx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jrodrcrc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3epilxkzb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kmfoqcyf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vcqtaogt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dqtovlsr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3abcypekh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mljokctu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bvwespgo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qpklvxux.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3isirpbvf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3urjsmnbn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3acomqcgt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gshbcypj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3exhoiytv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vcvqyhla.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3djkhplpk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3vsjyygzl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fykebxst.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qiligpxq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3rprekgqz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ttdmrxys.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cxxggiql.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xstonzsg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3iqdwaqyr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fbegtoje.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3iomecomi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fkjtmiop.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jaliqgns.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vglnxght.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wnjgsims.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rcctinzf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ujxmdqfv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bziytzpu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vthhsdez.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqbbbad.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pjaxdpez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrmnnthf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fdldykvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxeycvnr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ziruhcul.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fcutfrkb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3oilpulxq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hksdzchd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3txazxthm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3omebmtsg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hdjgamfx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cmauhene.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ojmagvis.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kixjorjd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ymvulkon.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wqlffqcf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dajbwumm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3aghzfdrc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ipowhfee.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sjiybtvy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fcqnlhjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ipdpbcaa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hwblhumc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fhukcpee.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xusrvmsk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mbwaftto.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kuyoqslo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xjdstnzd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tqumvjhv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vtdnkodr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ggbqytfp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wkhshhul.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3awwiabsd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ukjmbvwr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dwqqimjf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gmlgagna.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qzexgmlj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jxwdpszi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3arelscdb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vcjduyrv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pseqasog.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vcwhhole.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dviabzoa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3trmhghru.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tvmmydpc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pzuzzthg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yhwmarol.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kmnduokr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3drkpqdnl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3edvsteyh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3juxrzudh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uijjlicp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3oygtyucb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3elpbhoti.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gpskimbn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ljpunstk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wwxzpbbf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fmzxmztw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rrxqdpvq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vagkbxxz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jtwxmezi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qouixwez.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xtvshulw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3annwoajs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3azgdflmu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ziejrrve.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pxefbifz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nacqamyk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xqhwhkcs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rpdzfjdq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3czilwuku.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rabqzsjo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jvgxkfln.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hkylkjsk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pdfbbcxx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ilnedfbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmrqudvw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3qwkvjucm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsfgrzsz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fnffousk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3obdosgaj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aleflqti.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oidxnnjh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pteemirn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqczaex.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngirfhpn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3cwcnbtzy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zqljdglm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rqpgpidw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qfinsikh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rcgzrvmv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3twsxvrgw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gotfonbu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3nfejtqzg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vcxlbvff.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ahnbxtjy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ldiqtbys.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ahcgfrcn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vnlwkbaq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3opjshnwm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hbrvfacf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mlglmcqf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ejkffain.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3tgysanig.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vzgtfvpa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ezzkyxsz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lxoyenvq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qzurafxp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwxgrqli.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kquyzxyd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3deldbkdg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsvythcu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lqaevjgt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpuqeufe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ppoldfym.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lnxdmfvx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jmqsyegr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wakxhoah.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkyjxrac.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwrxdjtr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hgecllmp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vqraappl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cchnibgp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsknfxwq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kvtvqgfl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mllnubkd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zeupkzbb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cftyggye.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fmydpxoq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3bucqnyzc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vqwfzkmm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zjsbfngu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3soxugzat.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3znqxwmeb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bpjahsuo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uodrvbgs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vsvjvijx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3srsznakd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xcguoxos.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kezqkqiz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nsiedgef.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rzxiclzz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qfhifsry.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3iulesdgc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qezsaoor.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3amdpzvdr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3espqzbsv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tlfwjenb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ijiknvdy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ybyzgffp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nqubinzl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gocppark.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3toanoatz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gsfxwrkr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zpllrups.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tkukurgk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pkhamhso.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3smlgvrie.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fgjnorym.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lcpljleq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3clhjwfar.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bgznefrt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ipnvkqyj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rjbrmify.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ujitsldb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xmoahhse.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uulgutlz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gaapklvr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sltphjuq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pbvfmtmo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jurxierj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3txpqwhhh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3njnwzzla.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iksgkhmp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nfuspifj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3autykssd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ubouraoq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jbkeobsb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vsjmmwkb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tbdizycz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fkzriwmv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wlyxwbhz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rciystqz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fcotjrgr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mpfpllav.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nytfggil.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sacnppxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhnzuluq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wjshbvkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjvqcgty.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3djqxusan.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ezldqlik.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3kupfzvyj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hckcmjtx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3imodsrmm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3litposbf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3flmxyfxi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lvftrfzp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hbgmqmeo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ztzpljvw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qmvetjyk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vcutkhdk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xcixdoza.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3inglwutz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gtymnlub.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3taouedkm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ujkqoymd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hwsluqez.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zvwjkccc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wpwnvpvl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qzovesiu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jxtxhgzc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iwrlmotr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmibztti.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3byuzwkyo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kxpqphxz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zkujbuxo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tykhiwmk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zpoopljx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zuouqrqc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vokfddfc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywaqqsxs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vdtibhqx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rmzajmco.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3cvklqbow.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3amefhstd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jgxskcpr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3yyvkpfix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gkhaibwt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3viqvabhu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fxgdbgzr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hwprotza.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ftmhfjye.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3grkfygig.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jcozhfzt.html


<!-- 参考信息 -->