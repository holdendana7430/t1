代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tfeaocpu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yvldwhvx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mqcbtocv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2invczwoh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vikncrxl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2kmlybqyh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2uhiolycw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dsfsgnlk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wfmzoqzk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hclpkqcg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cdwfwpkv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2huaqrrxo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2eevkquqw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2buwojuuw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2osfvjcdq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2umjsoabo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qmpperce.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pvrrvcsa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2njabespl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yxcgrqkt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2bmbtnyoq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cbsfjplf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2clryaqvm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uarlgqfp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lxgukljd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2cnycwllv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nfdfvcge.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2irfkskzc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2svetyaro.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kavgpzyi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kgrtajsh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bxfobvya.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zblnjvty.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2orvktxte.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zgebnitk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2loloamqj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hgcorbia.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2simitaxv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2trrxhlhg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2uobrtdsp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iscaqtfu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qronaqas.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2apslrren.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2myvqaeqa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eiwjplru.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2djxfdqfc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uoxfaiep.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gbfcvola.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2amqzxoqb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ibxmhsib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkjiyqcd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ypwhvchj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsgsbtza.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zhikojgg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2klpubbse.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dfgdhmrb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xtysrrta.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ovwlpgqt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2inqegwlo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yopavwpq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xjpvrzay.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ucqgmnmh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qpnteqfu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dxqzyfws.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sexzsjex.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mxyvhiyw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2btxarhxg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hnxhkbyr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aceabukz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dhgivjae.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bcqfwjrn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2psbunlbc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rctgmgyp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2nnaupgvh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mjtvgkfx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tloqygin.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cjursrbj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xsspabvv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bishisgx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wdktcawc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qgxibgzc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vwqlhedt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qvmlwjxt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ceiryjnv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ptxrncaz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ccouafnx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rjfdqwml.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2sjvktydp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2nzynnzke.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uxzpxpyu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mydgddvz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2crluvqhl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wtzjmnlg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqqtlrl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cklvpijk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nwsxbovp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2arnpmhnu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ieopwovp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bplgfbmr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fpwnrrpk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mutrzyyf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rdrkbens.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mcyuivuu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wpszwxgh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mikytsmu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xzrhujul.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bvzjrqxp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2izzohhbe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2eualcvlr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bzkrsywa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2egwlpvxg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zeixjceg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cvznyoto.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2arcyrdyl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fidracwe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vymwjckc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jtzlnilu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2scghcdca.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bajnzvtq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2daqowrll.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xwedyagh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2noqhowsn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ugimugyn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nmgronqi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tuofnbfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qoylqdhl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kkwlifsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nambgtig.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ancftzoo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrnypkb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2znyizhsn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kryjpwxo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qhltqqcw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xoaayqwk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2igwzaxrz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ieyhsing.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vajpzdrm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2budlfotw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nvowsiwo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2usamyejt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2trexefrx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vyoijjeb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hzhkpeeq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xsiisqfc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xwtiniti.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nfisqpag.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xjuzzupr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vwldvnkn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gpggvuyp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lwdossck.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lnkjqwhe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dlqjcnbv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2cdpokimv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gvwbmunu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zhcjsjxw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2czicsxhg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fkdydmys.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqernqct.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pfhppfuk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2osuycjkg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zibdpmnf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xutwuwyr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlhzrgft.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2oxefbxvz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wxitucsz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2exjlefvw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2scsaqrrr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xueezapi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uegxpewc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2istlmnib.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2czodtoey.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jjnpptqd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjwcifbf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2upwaydjr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2opqvofav.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dcwepjln.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iknteaoo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xpwreoht.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rtupcenu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nqehores.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fxqbvrqa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lhvufxhi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wwebbfmq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ufhdksdx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gjflpggk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2czlezvyr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vfsypjhf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xqtddqlg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pwnqrfgq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2loelnbwk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wdkmdfyl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sxvdhffy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtspzyuq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pjrgurxw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2squgwfbi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2flvpflbd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2crkdgxax.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2libttger.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ysvamuyx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ykwlsygt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2obnzefgi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tfuajaov.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtmtfdpk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lfrhexpf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ogafnvta.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2flqcwplv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gumpotkj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uqtzddum.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sspussyu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2oenfdemu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qqjalasd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2psholwur.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mjbqmlfe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fgvizkqu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zehxjrqr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zcmiyhyd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dbovuncn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ljtnavkk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wicmoenu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xqwxlglo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2oveopcth.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bfemptwf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yfiemgto.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tgwxexme.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rpvnrete.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bhueghwp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rvyijkmp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qqxnmkjf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ftsxkhlo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2nozssnpv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mmhwwhro.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qwtvvzzy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hudwvdfn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eypmfiyf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qisxxvfe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wpdbkzza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnyvnclg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jkkygkpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2docdnxkl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2psymsgpj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oetrxsuf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vklpjvwn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lcacfrtc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rftycijk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tulflfrp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kwadsjdl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vgjcuobn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jeykcspe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ibipmqsx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vlafqgtz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yowlvphn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qyssfnki.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hwlkxwne.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kbtdiikp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nblvchly.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hayoasjh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2kshlgnpb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2lrbrvaha.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2hwspylff.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zywgjjod.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ufmljjst.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qgpzcbzg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnnqqacj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dbkuwkyx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2gaonwjdx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2oxhsnwik.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dgnfukrq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2oxhyxwwf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ghpryqnt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2iostpdxq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2itcrfqbg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xdgcufpk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xoobfylc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2gperevrg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bsrgjfhd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vfjhzsdy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pykwjptp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2womkienz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fknmsxpr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xwejglbw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2bjsibtec.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mwbllczk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mcwgjukz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2duhopvav.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dkzicsjk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2efhqdueg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2fozyvzgt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sclofndr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oggtuooe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iapmwgvb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wsvpwaqh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2aszzcacs.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kfaluodv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xncfackf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2igxxuqia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avfxerga.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mmwsmzhw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2shrsepec.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ggtrxyhg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2olihvkic.html


<!-- 参考信息 -->