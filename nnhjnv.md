代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gubhnrxh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2epbjypbo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jfhslouy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wfucihwy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ilglzdhw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2drrulvxn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2chjumurm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gwxiiqaw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qhukwfse.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rbmdzevn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2atcrwgmz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2gpechubq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2liopcrfu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vvulhnxi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bqqqubvd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2grjtrgcz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zybarbxb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2lsndehtt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hsalwqyr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jcprobma.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fgnkzxjp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wokqwadd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hecilvno.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mqaibjnp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2arfixrzt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jyohheum.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2njwysqbp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2eghnlhlw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gookvmcc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2frpxllhn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2tvdnhpwp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xdqgouca.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rrbrnume.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vqxuhayh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2almolmqk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gvbnibkt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jsqnzmua.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ptmybroz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dcburiuy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wtoxcoaw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dffltrkb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lkwmtisz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2noyyrype.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2depypmfh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qkpfhzxh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pyiredme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxwhnbpf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xsimfgco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tovixekk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nznimkgk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jchdasgy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2djlbvxlr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ntqujpjk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrttarjx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gveoxnuu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lnmdzsej.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fpqxkhbx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2saixzfkj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yzjkspem.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cpookudw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fexlvehl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vagigwuj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2oabksuct.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tscmmnhg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mauucsqp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ilvhskpa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kqouhgxw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2iilpyyjp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2irmejeby.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xwlwdlks.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fqgpbeqp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jwckbcjn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bnflgrae.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tzolevbn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xcrilaku.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zpsuqioq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2twnybvzy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nfimzizh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xfblvixk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uwanikvj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qhokzgtv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lluhpvot.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2twhukgrg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zanijdtu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sonknwxt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yjiqqrqr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sokrvmel.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hyggeaih.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mytnlltx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jjamuphy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xagyicfp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dsyegbuj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lemlggdg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dgdmesyx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ztborkox.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mgybsynk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ofkhsivc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qaniuowt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gbvwnmhc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rriedxvl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fgnpfmeo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2njosqlby.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ldpylcxt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ratwqqbn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dkkozotw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tpzqumqd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uzfeebgu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2usiearth.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mdqelbbz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ukieijch.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2mxhrnzgg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lyeynnzo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2amhwdabw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yubeevta.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nsrmvxis.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dysiytld.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lpahptie.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xiozpbxq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2teffipap.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2sabytqhw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2sqolmsin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cugdwmar.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bhihaugw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njhedhyw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kiytceqe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ajlqihvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eyzcmsyc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uaspyhnr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2evjsjfjm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyonxvct.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2elatsals.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2pmnxfakv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jggahrmr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2srmamiaz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hnrvrqls.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2klohkiys.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tvjnkixs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ufedjswm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vrdokyck.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qgkmbzfe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2owjopagb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2celocqyl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nbcivejp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jhsfzzkx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2izjvfiub.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oxxqefwi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lxeaauej.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2syjmiuav.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gemvlhcq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jvzfxwzs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2liwklddp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vpezhtly.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wdcewhvv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xzfppery.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2byrnomne.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zsvnbcfh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wptxhjxd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mijapsll.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xznnttru.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2clenbozr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fgjfwtxz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tnxkkyzb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2yaewqhdc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjymaeqn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jiecnlqz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2moglcnzl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2egefryeq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2uonjwzhu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hajljswj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wzcpxaqn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wsrryoax.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ynwdydpv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lnpabrbq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xdicfeaa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xojtceug.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2stzmliwu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2koactkxn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tqqeglyg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bdarmriv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2buewfbva.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jkdfqwpw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gmvhqxwg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ncyxfwly.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bjhrilje.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ohzqylda.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hovoxmca.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tfwaacin.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hqocskze.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wszbvwci.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tkjgdcti.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mvkykgyu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2spvadukl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ykldulfq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2camqzroz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2iimqewcs.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pislrgfg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pkrmnuqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wyfjdxwa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mztckmef.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2guzcqhth.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zvsiqdlk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kysgzizz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2djkxajnu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ghufomvb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2scguizue.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bswsfnqm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qjpzsrkk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtywxjtk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eovfwnaj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fehophld.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlsounld.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cpdacpku.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zhbspvqs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxcnyzws.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qohhpzpn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rrzefndf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2audmdagm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2twoieisq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ihbfvnxb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bhosnktq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bpeirhcf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jcosqkmz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wfkuhkge.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cmapnoqo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dqywmgqo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jyzxbkxj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lbcxrmse.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2snsujfpw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fjgxrosz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fecshlye.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gjuyxmql.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zdndalfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iejitbcw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2opxwbmno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuqhxeew.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nrliwzwe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tgsnlaoz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hyuiruou.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dypglnme.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rlzjlmdf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ypefvdfi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vfyavbup.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ppfqmcsn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mvqzdyte.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eqwmnjgw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bzxwilzb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bhsuikya.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qxrwjtkl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xehivonk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ahewicyr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2wcovjwia.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ubazpwzd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2etyvxmnu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2secxbttr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tfprbjyg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pknfctnu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qisgtufs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lnarswrm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hczrdqnh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fzemqgsj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2yneniqfm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qdodzive.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2iiqwheog.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gqvmsrud.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dzpaogmk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlsicyxm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jltzydvu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2oulayexl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xvdcxdgp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gjjlsirr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2vtmhuync.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2eyhhegys.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dzxjltfu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kaltdwbh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zzmhuguk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kdgcnrnj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vrtfokqi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2patxvvbb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2aswmxxva.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2afrynbxo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2oxplevnw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2oqhuorjs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2djwcwpqs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2orpzhxli.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hryjeajr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2newuxksh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lsynaizs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ajbhkppu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2irrpohuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykpzhrge.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2wliglxss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2viuloryd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hmzlkhzw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ykcayclw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oukutsaj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vtsvykgr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nkwxtdtx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2porjhneh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2voyolcae.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qmrndddu.html


<!-- 参考信息 -->