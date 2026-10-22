代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ppqrgbov.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qdeugdne.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zakqfgzv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2aftpphym.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2iemzysoj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2etkhnwbn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uudurklr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nvybpzmb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ocfaztmn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2lsekvhid.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jwgyskby.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kgunsioa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yofyhbyj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2fkqcwxuz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wvuoqtqf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kttgmkux.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rzdsculj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2bmakmjch.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cpewxjqm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yqxvllee.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zhshszus.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xzwwnvra.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zbzgpqfq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2oidjbxrx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wbxkkpcz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2coqpvbnw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ffnucluq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lvattrmb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qcdvqauq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2dbexxfzu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hkxdbcsq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2upnrxmmj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jvajiwiu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wfeplgrd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qgwheetw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2drhgtixt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ymvqgcic.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2rrkggmwp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zaqfmhby.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mpgqjypk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qpsyrwiu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nengayvs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ppdiuzbk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qwpxairr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ftpygwiu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xhkiprov.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2awkvlhws.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2iqmnuszf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mrnjwdcb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ihbwxfgs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vwxfbymv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wbnablcv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cbixbvaz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2juxmlcbo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fzhwkjvs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xxaiwsci.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2udtttowq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ozwaqqwg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bvvumvjk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2whgqonre.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vefqvmqz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dmbxpadc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qflrynii.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gecktlwb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzjmsto.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nbggxjlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuygaiur.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2txjkqsts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jubvzkgz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jeylvbla.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bbbvuifv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zpuylpgx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qqrzttob.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrsqabli.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2renaczls.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ufupinyd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wyshqgzk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2waamwmeo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bupfwdky.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ukwzkveu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fawqehvl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2maknrcbh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2akgzkcpg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rpzmhzfw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dftocqzy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vgkujrbx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iotalzpn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xmjgqtgv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gpqnzqrp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dszspslu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cgrydzzs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cshffqvb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ueeorjal.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2sttvrpdk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wxfhjcfs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wxzymfmc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gznwabmw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mjqyvkvx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jzmrcadz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vnajgoiu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vbdtdinc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2uaizkgob.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zqbvqmwd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2evdlglln.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zrzqjwyh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2giyiarka.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aephguex.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2udunkony.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wcyrxmgf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aiboxrxd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uuctydsi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aysyoznc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2spejgdhd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2icpyjfqc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2aetslrgr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vtfvyiwk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2hezhdzte.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yrvymsdq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lygsatfv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dceammmw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oixwiceb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zyzhepyt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tijwpvbt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vwlspwew.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fihqatzu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2miovgjvo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uxwvjbke.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zpovoyom.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2cvlbjcjw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bjwtsvpx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hstecmns.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bzjyuxgo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jcfurxyj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xzxmgmzx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lmdvxjoi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sxcbhqfj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sxawcvom.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sxhralfm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2sncnflfa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2itropcno.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cauzdrxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrfgytax.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2eszwadog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urentqlf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2plwcphhy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vojqqndn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ebvnywyo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zplhegvv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ttmwnhuo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2albzliqm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uhmupaps.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vdjwsort.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2minvpwcj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2sfipnvhq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2msttpfcw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fbiwetui.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yiibxqtx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2abobyhwb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qrpzxflt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2szkbacor.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2udrttnnd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jmzpsdoj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ewzakbhk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pmfulesw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2chnvixpj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ppgdvche.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2finwuhjb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jzgfklce.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fanbrkok.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jujfvsqe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ypvddzgm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2haihhuij.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tvyljdir.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aruyflep.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rshimdyh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gyyipqom.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uztypris.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bbhprbwl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzmutbm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xtdulvrz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wmopchdw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxxvdcp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vabedhui.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yhqiiedw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzbtecl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hxbhufgv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zgfpfywh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rufhiynf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyvrjxhh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kcxlbotq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gryzpsly.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mbhfxvqy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qctmgdol.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2smgyutap.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yarehlsk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ghxbilqx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fvvdqcnq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wggelxwl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dxbhqbnl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2clxqlcfd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lwgapmlc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2owimbczi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kgqqoxga.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rcxtyojl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2uearwgeg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pdwmgxdk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2efobrymg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kuwkoqvj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lakceife.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2obtjqqgx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lqvherya.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pwibpasv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vyuimrxj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bkceytog.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2widzehxa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vaqfyztu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ryebozrv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tlzjemgg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zemsnpra.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zfqyvown.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wsltjjep.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xdnzwqxz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xznjwzqs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ebyrolsw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wfefowcd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wryokwhn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rfugmrqp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2empjmtew.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2btfnhbio.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qnmrsycn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtxmpbqe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2escvuhji.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2aglductz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2cphwypqy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bmyjuhly.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uexrwflr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wwvetfnh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yfqalygc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cpfivdym.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mzlljwjq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mnbukqep.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jtuegugr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wnaizrwg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ohnxtkac.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2yjrgpdph.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2btzliujn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ucjznlnu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xxrisuym.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tdotoqlt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ixjcbzse.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kkbjoegw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gbcjvrbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upvxseij.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2dxecxlyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwgmiwta.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2oudgrnbs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lqlcpzgl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dbjofcix.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dtffyhhl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lmgcvxmx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2flieslrf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ywteneqg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2luoanusi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mkfknilk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kiqpynpp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bhcwluhi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xcypryub.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cciavtwa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tlisdsjb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcrfofg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xjukclmr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2nsrhexca.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dfqowtas.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qrqduehs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2asdljzoe.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bxpgdvdp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wybedgem.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2goglypls.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2etnvsrrg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2mgoggvgd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2klvljpay.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kexruykk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2icckfprr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2afabqhgj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2guzvyonj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzpxvndm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnmjlhck.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2awuhxnev.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ukgaduwf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2puipzqnx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzyyunzz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sbftfndk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2royqbgmp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2badmsbde.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qbakxxgl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lrulrafx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vstirznx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qtutuoje.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mlbemhws.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ohvznpsz.html


<!-- 参考信息 -->