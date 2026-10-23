代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ordfuadd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ktwsldrt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jfhtdgfp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lqbucaxg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jisrwfoi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yblnuswa.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rsrrmtgo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3msllawkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lqhuorhw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3snugabrv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ndhhgbck.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3oifqsgyn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vbwuvbji.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ocahvzax.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kgaqubhc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xbjidjeb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ohyzeqwg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cpuqjigk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ugbuoqal.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mdejmebv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdzpknr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3afswzqxw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ntkhmhzp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jxxgmqxf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3oqfopcbi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3kxqgvohz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bbfxgkml.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cjloywbf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zpiezkog.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ciarnbdk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ndafwpei.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3pzcpoubr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pjdapzwn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tmvgtvis.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cpwhqdso.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rbmsiwym.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yzizansy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ebrpdpgt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kjplqwlb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ydqawzsr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3prfqgaqw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dgiarjsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxtebtrx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3smbqavuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzapygzg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gcipgoch.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rekeojwv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3basnqwzf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gkkkpmiq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhxzrutx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hoklwiuc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zdngeufz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hegxlxnp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3abbrseld.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3foowwvxf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pdxztrfd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tgzzyhye.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tmmhvjji.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mramijyf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3olzimhxv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jbnktkwp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3twpouxxt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ipbcfnzg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ivsvbvcp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tohufsnx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3biayrsry.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jouwexka.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xwhmpbuy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ibdhknyx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3otabynus.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3whzvjzey.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qsqhvnvb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zuggilxq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qbkzjzqa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xppdsktp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xzqdiafn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bkydxgmc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3oclxwrwx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ujifrmdx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fczkzcyt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3czketsdu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gdxvizjs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cmcxztku.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tyndlnci.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nfxbgjip.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkhvijip.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lylplyfc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3emjotcwt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3unegdutw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3iqbzfbdm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3kyqpoiab.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fmiokpmr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qwomhgqm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ecwfawfy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nhltmmpj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bbhvajvw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3todtizty.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yldpaefd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xtgfhlwj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tnvtdnqx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gwwwxayh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3oafhylfa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fwpxebno.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qeobmsau.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wekdymjv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mmrdxqqy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tjwtxqej.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qgodeyok.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wwamavzj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xnezahat.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rdevjumm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rzrmuhdc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qzrfovxr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zcoevpzr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zrlhsiku.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3awevruik.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lfxnkwpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbinfouq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3svdbmuln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3neimuelu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ysplilox.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rfcmgzvd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yackookc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sfuqpigy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3glhzxxmz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wxukixfj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3efobxrbh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qlauewxr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlddzkdp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rahbzhhq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3srvjrsqx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tpfrfeig.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rdpjutbi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lknhldqy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zixlryrm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wsflgrrk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uxtlryiu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zqvvhlvf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ocrvnfzl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3pbvjsrnb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dnhurpqb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bivftwqk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uyjihesl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kjhswjuj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jktfboze.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3uajrbioi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ybcdwauj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nhtkjzxx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmxcuiym.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdvrmrhm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pdrdbbgb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3arvdqnaw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbsfmvlc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kjwepkgv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bnzxvtfs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ktvqcgho.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dmyrlcke.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3amhvdwad.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jbdbzhym.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dticflcj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecxxmkqs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dnflaaaw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fayncick.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cicsnxrw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3wrymrotm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yoyaiucm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bptcocia.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tngrokfb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kddfsgbz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3syevzjzg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3bcmyhybh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3otakzoqt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cifllcfe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ygfvrgii.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rospkcwy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bgtylpno.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dswievzv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhaixtg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3pnywtaoo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rgpwqmin.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xdqucjkr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ngsuyjcc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3buacjric.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3unhlyjbo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3skglvazy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qyqtuvgc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qckwaiyl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yeeorxsn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fhagixll.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fsfirbnc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3axnzkgoi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdxcsqjk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3owwfrfcx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rbskezgd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vfjirmgc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kndwhhnw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3hudbfkrb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wniylshe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mwytxxvx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdlevgfs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rgpzthsi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fsgnucsv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3czxzwnpx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fnaimgum.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jkurhdla.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nxjymitg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hwejmklc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xcfhfrxr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wbiazjwe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3otgymxmh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3psexwkrj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ykzsynbu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3avvsjnlt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3djqhrzui.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jphboouj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fwmubbfb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dheqyjbn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3rdoyhlya.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kwuxcphk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3sxrglrcm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zjazhkrn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vxlrkjao.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vvwdfjkx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wxbznnxk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ovyexkrd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmjmnqn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qcxaftwx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nzrzrjrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpwdcfqd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3anzzfgkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpzbqxgv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jvteibxs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fafziwgr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3udriysuj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zscgpcdg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wvuoskqb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3symysudc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3drqblsyk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3yczkkqci.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wsctubeo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gphosyei.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3uygospxl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qglkrfpj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nstzsdro.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cznhyhwq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ubywpxid.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hfruigzw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fxdpsiig.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xxadoppv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dneoqeqo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kuwpiisd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vefvhjdx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3otdabkhg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ezsddvtz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zopbjyes.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gvvywzra.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3bxxeuyon.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghwtynrw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3oqdupjmf.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3falckbjk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ytokepmb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uptavyos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uhjxeypn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kdilpdlm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hwbwxxne.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3otsmrvzn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkzhdlmj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nkwkrrbb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ufhvxtpa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rnimlkur.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kkgemlwk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ljviusoh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vtiwnurg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3calyqmce.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dliyswah.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ksaacvwc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3hpyrosrx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ufoguwvr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3bioioefn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3czspfhcz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gbxfagrz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3blzrpjiq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3humwqhvj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bhjygeac.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ynvsaltn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmwlfaey.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3bchgyeua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jrtcgqbs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rdeezeui.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vnhcstma.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3foxczlyz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qshpfjxj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3myfllbvi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ezeuefis.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dcyyvrgs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fbvvdrsr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rrwcuvwi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dfqfxjba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xhloycum.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zoffhisi.html


<!-- 参考信息 -->