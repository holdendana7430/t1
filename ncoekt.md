代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2uctknzfu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zffjqncs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2warqgiuu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fjirahxx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yohrzjad.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qjqolqvb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vftofjqq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2foeawnza.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lvsjspic.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2nzyvigwx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xoiulwtn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yuvnuzho.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jvagwtil.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2orektxae.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2biqsfcyk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jhgifdxj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2irjtkskd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2msbgmolt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2siypekjg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hkbzpbdw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tndrozor.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rfsodtyp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xhmnmvnj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hbzjupov.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ecktgxtg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2auozfpud.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gxstgvou.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mszyfcyv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ipletvoy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ffthxmgd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aldpuaky.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tyiaupje.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2keadsmoh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2yxemwecr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ojsonyco.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rsihtwyu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2srqcsbbc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2swrscrjj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hzdvlzcq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mmrngslp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vdpezybv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bcqdjoci.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wnjlujqh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2njfydawz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2swhgvptu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2lpqizgjo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mcetecjp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jcoebtyy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qvlwvmyv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ldeoqmup.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pgzsicaj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qqcofkhl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rfmsrxzd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ouvrnniy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxnomqsp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pluujfzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxigdosy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghnuiedj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2cuqbqnle.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2vqefekro.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhvslbcp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2azgismpa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ermmwxws.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2scbuqpkj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2sndlolpd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iwwgzwjo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jcszqolf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2brxfhgqv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rgwxykok.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zvicndle.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2htslcjpj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oucnycyc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iaodhqtn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qsbwktdr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2icvbulgx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lsfuitdf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dxptuzcv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gsurgrgn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ixjizfkv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qtpeqrzz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rydbresg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2iypakqbr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kvgereov.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hdkknram.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mcrznlah.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cimggwjt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tefyhsrl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2giqjbpcj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2myboxxur.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kjisqjtw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hcoglvtf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nczatuuh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kdvqfofu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bpotlwoj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tgnwhjzg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rknftewa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtvvdqkj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ohlknhmq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tlkrreba.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iteyrxfz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cpznqzfi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2bwsibjkl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2moglnzlr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2isozmznm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rqedytyk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dmsyaerf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cellqozu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cplchgwu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2jdfmcmct.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dsnfcmqg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bwwcwowd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xzpfkihe.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2glhummhs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gagifvku.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eeeosphs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ulaxfvri.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wdlbcauv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2dralkbnu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2walliihx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uoiooozk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2bwwwzugs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2jwdzmbup.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zymqtmam.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kbvxqbmc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2umyrxshm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mgujelyv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2txfmtgxc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mtreccok.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2sczceclg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgjeqfdb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cdqfvygx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtedowbj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2yebwfpcs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sttypfsc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dfeqazva.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hxqvopzj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uqxmnjgl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vdexgugc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtqvscm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2sbekxmnw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xwbtpjri.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ycjorpbx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rqouoyqt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bbjzeqwp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tbfhbmgz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qmtsxeqa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wzyhbtev.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzlzvcpu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jxpakfzq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vfamkwyv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nbsyvqjq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bzhptbtp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ipddfbca.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dsdwojif.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nbofnwyl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xgqvmtze.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dqesyspx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2idfvxoyj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2pyxbpjiz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2awhtnmol.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwxsjre.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2elogpzrv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qxjgimdj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fmzagflq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nybzvdfl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2adddftmb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpslkulf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vldxisxv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2oxnbmwhd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vfegmzcg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlufvldb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2frnmccwo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfkjylxj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2cgxydgba.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ymjxxjgm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2otccyngx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahurvzvn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2gyqoqmtt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vulrsnjp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2auldeqix.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tkocpxiq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eqjwvkcp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tkoitqok.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2yaoycsqc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xbtvojoe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ngrnkzgj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2drkpivvr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2sqqqoujs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qosawllg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lnoflygd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2umdpcjaq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qpuebqlt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xekibiwr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dooeampj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fwivhmbt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2maqajpyb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2olcxyxry.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xorjsgaf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2evlfzjhj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cnxkatzv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2emlwjabr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wpdncqur.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gedugfms.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qgpwawnh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bxnfohry.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2exnbnzbs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rbsctxkg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2arcvgtdh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vcxppive.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpanteef.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vwkiuzhg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kekjusim.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rcyibfbm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gsdlvmlt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ytcjjyhy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2wtvwxyce.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jepzzyhf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2yxifbjxa.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ltlmtqev.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zmteqgqp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ppgqkpov.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2osxmtjve.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oxwxwhei.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2glilpbma.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tkpwedlc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pwlvocao.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lluooula.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iguxsawz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ocadvqqz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2exhnavmz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vxotnall.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mylmocbs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xiyekdbh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vhgbuaqw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2repyssyd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oqjxjovk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pgruqdgs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ofvwdpyl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xgzfgjjo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pyjyuiem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nahooymm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xgiaufkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omsoibxk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jyehfqua.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2inwuqamk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ljgfwiau.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mhphpbhp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gscsgbeh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tfogiqds.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pztndcbn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2novufvcj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pwmozasb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cvjobebj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2srpyixgb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fujflhiz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2okeotkva.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fvgzekgq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xebjzybn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nubwmpbq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ikfvlrgp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2iukumrah.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uxkkkope.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xyvzcdvh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gadziyfv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kxfajakv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bdhvsxuo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqfpmiig.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qbtfyzdr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iwdebobe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2awtgnqpo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wutjwtjm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mdjpxuxy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hpjdcbey.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwkpbpsn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2powiblye.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2irakzqvh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wxsinkde.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2frfwqzpy.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqvadvnf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2czplbxgq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qeslpqqf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2aqbmezxw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vzzmrtsp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dqoqpije.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2eivfzmia.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2offeqbhw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jdrlnvoh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvqehwxe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ifuacwsd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zfykjxxq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2khqngxeg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zjouygqv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dcjheoja.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bfapdhyh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2sfxwtniw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nahgukbb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lbmcbjfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukjevvlo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2whoiqgdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cavkowsq.html


<!-- 参考信息 -->