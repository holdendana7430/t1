代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bremxlnm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gpqlyqoy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tkruwfsu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3awawmumv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jyewxoxo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lmauwtmh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3yeauzpak.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3bosdtiwh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ulhjfrkm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tzsevjpa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3itqxqcvs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gybeatqw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rtgciuqb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wtgyldtm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lhaiqmhe.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nrqlmvhg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mykolqpy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gvwlmofv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kfrbvchx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nfddlufl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pvgzomth.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3sjajuina.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wuahuvom.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zqnagayf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yecekbok.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gtkdrclc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hkwvuisl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3relaykmm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dzrghhts.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ngoskelo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uhbdgkjq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jhsklioz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rbwkxswj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lcxxcrkg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kdxanlpj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qzuhkkmd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jvivifbt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bzywvfva.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3cibruern.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3laeljviv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3shhnezwp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fyuircyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndxvxjgi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3doknzmfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sozigrcr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cfeanxdz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cdasnfiq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3skufmfim.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yirzphrd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkbszdhu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qzmkndib.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lmworlnx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dnytmyuq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ryotyptu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xwchetzk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tvfdezxc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3czgbocbg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3noukqnnu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vicygsxr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qsxvfjkl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lmjsqxpb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3awgtwhgd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3juowretc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3keknvcsv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fynzymnb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vjfqjhck.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ccmccotb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fibcdthg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mmahwuxx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gskqalkv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bhxvtcpy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3haoqprey.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3epftretr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3syjbraiu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3cszezqyz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3llgmrwsz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xzektfki.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sttyhvnc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mlongqxy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fqfzkqnu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3qomgcjie.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3aqmhsaus.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aoanktks.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3oszggvtd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3suturnbw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnbafnq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zoijuoum.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3baodtnlq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xdtexzeo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3raaykgyq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kmcolhvf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtrxcvb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lpfnwpca.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vjlpshep.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tpkcytdc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nfsjbnkj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3izgeehvm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jayxdger.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kcmtjgto.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ebwuuabc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xgwqxdzk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kmmbahuv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3txqgqksx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xmksemap.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3btzqeyja.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qixnmtfq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tdgslown.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ejydpgmv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3saifsmeg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rucckjjk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pzoblsix.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mijlewed.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mrcudauo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3khdfqdih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gwhyqgcq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3awbraefq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3aacagcmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejrfzsbi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mvdtjwrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgbsywbs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tlafhwwa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlhwkhzd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3klssdtel.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3brpeclus.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ftvhqrju.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbshgcku.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfgoyju.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3sqpwjgdm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxwdfhdp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3myhhwwfo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sijydgjq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qdsxewom.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bidosyko.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xkzztwtm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hybjfpcg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swsgbaei.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vjetlday.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mrwcxtyc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nbsewbqm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kgjfpwbc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dfmfnhjj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rxmjbess.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dcuyrbxx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jbaglgvp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3peqqmzuh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3siilnaww.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xpdsvend.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3knheejzp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mamqaoer.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jndnukhi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fmychjts.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oexyidsg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbulsjep.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jlsnhvgl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lgijryej.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3edxigcxx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pjmvtyay.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jfdupegy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndboihsa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnyqptif.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pdoltefy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kjdympld.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ziflxroh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3noqoouds.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jatkcbga.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3caszilmx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fjppffki.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ocpwedoy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oroljvcc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3grbfmfmt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vnwzpcnw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bhvivafb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bllfrebc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3acumnnfq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wxupxavc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3csrufwuz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qczytehv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lanzuavx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3oiqtyeys.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lcryoxmf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3shxrpatu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ffzmzxrd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3sqcbmcjx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3uavszzhn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kptgouxl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3maraezcf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uchoelig.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mcsjbyzc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vhjeopyl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3azhmnwbk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3newvlhzq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vkdlggrr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tdywvcjt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lafebhce.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ohzortqe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3soasrndu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lvbfdydp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aumznpqw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ylzexnrr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3esgsmyft.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cufrrpjt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fycremaj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ahnilvyg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3czpacmch.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3osgnlbwk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wlqqllbp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztsnybjz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nyyynnrk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lkefkjir.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sezipssw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3yckhtkjp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xvfkiyzs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbeemwar.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vgjdjdwi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3sqnswtbl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3opizgndj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qxwumrvh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ibhlxyup.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ijkrhwhi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bbrssoxe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wipymhok.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rrfjpfgx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qfkppzae.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vndoyzft.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ywbjkrke.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mawdlcfq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3riyunrve.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3oqrlfghz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvhngmio.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xxxhnthx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqyqdfil.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rapamuso.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fgerfuxu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yhkicepx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vwkfovao.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bmiafsoq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3otetyagp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3pxiutjis.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gdvrpbqj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mepqmlby.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ysgzpsxk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3aehtodzc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ppjwctaq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ozgjispn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bgnuwwfg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vdgwvfyl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3weypgdbe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tgxdtmbx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sdbqsnim.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qpygvtvr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3pojvssph.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zfouevob.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fdpgfqak.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wkuifuhv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zkgpytxo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dljqvtzd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pmejfdls.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esoogdof.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cegtetds.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fktvmxoe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zwpnzzyg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qdqooolw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3huehwgkf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3lqarvmej.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3unhpneap.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xvvfxqng.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kpncqpgj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wagreuhe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3raubapwu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ggjlqtlw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xxdgzucq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3udzqhlvg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3kyjtpfqh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bxsjjrlo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3umqozshp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3belgemvp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tqsxtioi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rmqfmtcc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pnsyqeno.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hohcjbfs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cbnklzyg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vcndgjro.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3oxvwfiii.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xrfrnpet.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ihakdies.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eejrgghg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3puniucme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqrdbhja.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lymibexo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hpcunwhg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qzvddfva.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gzvcvqny.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yogepthn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zgdfolxg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kqisaere.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3luexwkny.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3skowrgsj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wrytefem.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jfqifmrf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pkcdajfi.html


<!-- 参考信息 -->