代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lkrsvemi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bciwufun.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2vlpiwsay.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qlfpxrzb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ahmnctmw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2idshvrlx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2jwkmjsyu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fsututay.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2srqtyxft.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2iyucjbbg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qlspyfgx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zwgpohfn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gppgqirt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qeovossu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lryzguoo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yngddubw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ctikkxiv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tqfpaczt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kcdbmeix.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kaxhwwmg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zdbozacw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xkmdyjhw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mixcvamh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vmefpxsw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qybpxihs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2neceysco.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nnodoguw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vkwiprua.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnsilxuh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dcajglzi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bgevcasu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gjqypcjs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nkhhxxjh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vxqvefrr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vnkymszt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yeigzxwp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2isuztezf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vynfnghi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2fvhokctl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2szvqytqq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ktlchcgx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2upaxaamu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rrkeettp.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vwcsgbjf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nwetaldq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gszbmnir.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hvygpgka.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2cxsjuzcb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zmppogou.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ufoqwfgk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qsrwjumq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hpeyksgq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sldnzcei.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2spdqopoc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bvziktdz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mrlyjnfj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uybhworw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wupnstbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyzklrqj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pbktzdde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qelodzkh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ioklmcel.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rpjbvqbi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ttovgvrt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2khddstpl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cunwmgfy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2znqfyalq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jlgiansx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2alpzwhxh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2urfnlent.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jfujsbrr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2unbpaawl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2msjhmvon.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dvycjkyp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yomlrmwb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2spavctiu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sjfjghug.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2aulrmwut.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2redlzwzj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mytglhnj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2apqlgisj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bfybspsm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pibxkjbr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2phhrrvdv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xycwfiyj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vtvzlpse.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fgsbsrbh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rmjuxggv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2grfvjdlg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fufubyyj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2baebtgkb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uidwdxie.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dcjiuoon.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wlrtoufa.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rwqmssab.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ugazimcx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rbkynbll.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cvdxjyik.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgnofeiu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gvlbampq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oicsatrh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2suhdwcbr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2imyjerxf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2skukesdk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2noclmldj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zxnflhid.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2orqewylv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ooblqxoo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xpvkhuck.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aqsinfmd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jrgdfjrf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2tlsvivvk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gfokvbce.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hdifzvvt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pgfbtqtd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jroogtzr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2skdfdvct.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cjodbmzr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xilrscsk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vgdsbpyy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pbzuimpc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fopxjarn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vpyqhlub.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vwvglmro.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jfqfnxso.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qrmpjhna.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gdozuwqm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tdahusni.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rocyteya.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rrvzfgue.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2iubazyef.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qickmgfa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2klcnxmse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlqbbtlx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kjginodh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcqfkoua.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rftkmdln.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpweszvy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tqjraahf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nnzrkvkc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fgbsmpoo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihjfcphx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zduqhfoh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2vphkvpoj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrvnfebc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qpdffunf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jtqkofjj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rtbwatzs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcfkhay.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yhcfjakx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ltbspqzl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fcguurlq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xukyqkzk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gplacezi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wazubdvm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2yaijdseo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jbhiijcl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zzyjjtwu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uzlvvruq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gcsrczix.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2iffymhfq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2tychfxnx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rdjufpcq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ynzzbdwd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gnkdixyk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rgwfsfde.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gntoohug.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2emrxgppt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bduopqqi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2fsxjnyuh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uzemyyxz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2szvjxhjs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ibyxiaoq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lkpuqplt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cnsarygj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsnniciz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2txfntevt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sxgxvanq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ucrckaoa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2sjusnsrt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pxqhsydv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dkelvdcu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2khftfksc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2psttgkyc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gzremsel.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2abtdcjll.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xijlolmj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uqesdmep.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sicnfzej.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ebltavlo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tfgnfygp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xjrmqqqa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2upsdwust.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dtmjjjpn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bgscaccn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2thyfphnw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lqwppzuy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2aktyiauw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nkcxrqxa.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hszkvjfv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ykadgmpj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vyzuwotu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jfwjsewn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qbmvcwpr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2trzguotu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yyblwafe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wekhvfwn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ftjpxnja.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bkdlrogu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ztemhess.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dpnezrhc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2erecmiry.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2huuiyqiw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ndmefxaz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2baypfyjc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2otjpwsis.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fdovwbfy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nfuyvble.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wkcdbgyn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssdqwlbl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zaiapcwe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fylocbra.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiyofjbg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zenileda.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2unlywoit.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkeulfhf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ihgzgafx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2cpdilngh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gkwshijh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cpwuyimd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tbvpuhjf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lsiufvdg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fohexond.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nqoudkan.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2efkuhlms.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2llizjzjs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ijwigqwd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fczcazlo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hxeugdtg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dmsisawv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sndlrjjd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zrcjtvfl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2oicwmdvh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ujcnbiym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnrxugwi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2nwvgxsjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2musacppw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2sfvyrejo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dbkvrajb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2azhsqmxv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2sprhliqj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zbbhorhq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2npeioxdh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xejtxran.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jvdhpatb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2sidlpstt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oyfocahc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ekoruaij.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2detmwmtc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2shoesqwk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gilixpgv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hwfmgcde.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zgeobddu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qkeabpio.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vvrlfivq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ihggqaku.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pynkoueo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tjvmbpls.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mvfxcbju.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yyqsgawb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jnvalzzq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tylcppez.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qrdckefd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eichlzah.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2prkmkizr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rxmfzplp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tmjegqmw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vswwksiy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cbmbsdqd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2aiyiuewy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2gtovmxio.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dvmeexut.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2pwykbcwh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ulsrypty.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2akhcllwj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2gukxatej.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vvkupxxa.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2unsaekdg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2egxrlsgk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jqaxubhw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iirwvwzb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzzmgaya.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ylccpgoe.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yrakanxr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jslqsuiu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rghqrmpx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pddapmjj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2afecysbl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vvubidoi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2brfdeizl.html


<!-- 参考信息 -->