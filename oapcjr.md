代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fhxcqqni.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wzfkreci.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dxluxxpu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xfgqruqi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3oisezafx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rracflsv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3tmvqzvzt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3umcwnjaj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3awvrsgbc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ywzsklqc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rjwucckp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3iwxgkgdg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zunsvpic.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3tuzlkxcb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lhgpqxll.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3uzqswgmw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yilsnqlv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bqzvwzgf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xzecwqmw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zzxavztx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jjpueejb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3psuiofwp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3aytnjqcz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yobmkuig.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kmupdqkv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ihyodvqp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vlsaqjih.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tacugzks.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wyrgdbmz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ecjbhyhl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dergoafs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ldrsztso.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cyopyhrf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3oayzebjl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3axfjtjqh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3svepptpe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3imqikygv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pnxnouzj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ponvqoqp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nglrysgi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xbraalox.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fvngqrxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaxrsium.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mcbzkhej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpqilnkb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sfmlopym.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zpbatkwk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hnyopqfb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3myqwlrqy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncoiwvyw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tiwaoury.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pnfovdob.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qrcezmqj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ghymppht.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkeaiddd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3twttnsih.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mjudwdkr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cvxsucpk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xitxrtyf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rwybixmy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3izbjltvb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jdzhyhui.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3trzsbkxz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wjlrukki.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bacppbqk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mevzltyt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dzyhsbkx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uwzcamlb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dezldwat.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xqyfkwwy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pketqzel.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fhcqftjx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uapgtvye.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ygxytuss.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gdiizuyo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3djnnbztg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3neusqhby.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3typpdhqj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3irjlkmkr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jqmjndcq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3aijexlen.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3emoasoqd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oztjurle.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hgkrlbxj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ieneolrr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3naogfkfv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sidglcvd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmzdjwzt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3aqhkfezm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uzpthkzc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pqttknso.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpfgnqxo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tdpbuhyc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vxxbcwub.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lyfffkrf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dfcxbcbv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3owasiuev.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ilxyfeec.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dppotqfh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zmkvhedk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3knxyxusv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wsggiemu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3erdjhfat.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uvwulzfm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3iltyenbf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3joqljzgx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mrlcdcki.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vsylzqcz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hfuuqciq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3atdwexed.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3iklujexe.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ajsjboav.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3umpifebe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rgpdywos.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qpacxyhu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ehswoxae.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gshrsbbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epvkzwxw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rztxokql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkasjcqa.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xafxripr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xlgozubx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dufcvagk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kllyleyk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3joewyqst.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xztabhrj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ghxcgppp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3cszuplff.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwmkzzsy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3eadwnhmt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gnwdthtu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pmceeygv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qixqeerz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pbaiokbu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ldhoppji.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3aabpkrmf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3iasnffqt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zfocbrjm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hioggcmr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qoddxjfg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3igmdzpbx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yrpzojng.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3acwbbyff.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3chbhmavk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wiskxdvy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ultccqcb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jrggoxpg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sewhyzxg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3byiytjsn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3huhpdxzc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fqhpduua.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wdfuviww.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qjnlrpzu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dxiojfnm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jbfzgtef.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vgqabmui.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kmmspgek.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cswlqwdf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3piatkdmu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxjdkah.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctekjmlj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nnmjlfgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bsvkegnq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pwxhwnhk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3afakstsm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tfywyfml.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xjohwdgz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymldflyk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qieuybwp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lpnlqddy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kewxjcys.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mkwxfcsl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ksajulfe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hbwwkevd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rrdioowr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3uhxjaeqc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3otfeajmi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gtraafvo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lhmndkhf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ylbgcswu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gyvovywm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ltkaecas.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3abhlxusd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tnehmgqe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cpltbhzz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bdmwgacl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zwxpvbrr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ogdvjxlc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hklsnpyt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wmukcvlf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ymazonfo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rznxtaap.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjwdblrr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sngnvkho.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jigmhfgn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sdzxhaqu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mrptmkfv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jvbzzyis.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rqtluecy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ynxckxpl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ojrpsojh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yrwejemu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dkmriewf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3xajcekyc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3czpuzfsm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vekernmg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3kmgdtzwa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pxntqthh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3furqxmpn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3cegfvkca.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bixcmszd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3cojpkaho.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ivfktwft.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xgqqlnde.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mthyejdp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vdgutewe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yzblceic.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qlfzostj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cfztbvbe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kmqyocoe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ldbingwu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3cwyoutfq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wohiqwah.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vvezucby.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ccorhqtr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3dbkmimeh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qnhdvsnh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yrwifabl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzayjlhu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3jarljwjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clqwugck.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tqephmch.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fcanvesk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncpctrhu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ljcwtfdr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gfenably.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hatkdulh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3unfezpml.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zpvarwzg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qlhvlkxy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pmhbnlct.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zrulqaca.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mvlimrhd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sbdsjxgu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wxvvxufw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fxtxxlbv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3zhtyexaj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3emgvtfos.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3eprzeind.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vmkzanbu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3olcmzmdy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ccybfujz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3iqjoimiv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3obkmhvzp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iujsnyzg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3curggavl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nqjeqqul.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdfghgro.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dutwwace.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ybeweici.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wyrboehi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bfihgkqu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eshctaer.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kxmbzrty.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3amqjlyrx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3giexhdgn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvigdima.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wzwbmqbq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gbuwvafg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ylajpqul.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3optesciu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gsuxikoz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kpnrnfdn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xxljffgi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rwzvuemv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3gilrzbjw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dbqymjbr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3yvjotrtp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rhbblrub.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wqdeurlj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ooqnbkrk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3goeueyrg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rujychxg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uzvqzchd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fvgxxduv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkqaswfs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3huyqmazr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrqgbmpw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3swrppqpg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kaasyboo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kdhbzujg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mzhppdhc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lnnfsahd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3usfikfri.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3igwjsqgg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ilvtfdjp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fjkwdtdc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cndzkhja.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tnmgauwl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3comxdnoq.html


<!-- 参考信息 -->