代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ucheadcn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jedfqfrd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dddtxpdv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xbtipvhg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3funeggjk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rrevacyq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lwqtpobv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3hqjrnzzh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnygcsjk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3agaezzwm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nkkdgfzd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tqnttexy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vskicgco.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gfjycazi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mbttqwug.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gxqbqipx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rsvgruql.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rpeqjesc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rudnjhxk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nonnrlpx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nyuplmlz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lyzqvawi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lbmpxdux.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xvqptagp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fnnicrmg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3bcgphuxo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sqnbgtga.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wttoxkoz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gkcdcjjv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3kkiupick.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rlkmofsy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zednejxd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cqiopyhl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nvqphoou.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wbtotciq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mntvmaza.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eyihlcsr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gbtjcyhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gaomxakn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jetrlcca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uijujspx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ikylzxko.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pbijirfq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3lljkomhh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3usxowpdd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnagqkrh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gttlexzh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jgnjkaxd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qmqccbzq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ugquhnac.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iicsbxtk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jsgzowyo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xzapggjd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3updvsjvu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xtgjlfbs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hekjypst.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zjwjupcb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gskhfdny.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fountswu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pkjhgsrq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kuqzpthw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pjyeesgu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ptgzmvwx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3abvdkadt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rzkmgeiw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3sthceski.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rzahwmjl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qpphrbis.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gjhytaeh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ecqqxmag.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kekjigyp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3omqfcuig.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tprchdqg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cmusjqxh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jmkcqskp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lvttuywl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hghemwkl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lpfxpqxv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxvltomk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3emzqbnae.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xlecwrbq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3famlbtam.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dkmgixae.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrthglv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jeuimdnu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3quazpedg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lciatxdu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3faybqksp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wdvmjfun.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hhpsaifh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zoahutdw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zgecpstr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kuetmqnz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3stdyjmio.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zltixnxj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wqssgnne.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3oyxxzgdv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lejtgjqh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yhqqnvik.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qxaumbcm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nhiupvbp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uoljdbwx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ccivgrzg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wubuwdpg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3myaimydw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qxdpdvsf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jvqposwa.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lltseijd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mfgeuoqa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3srffwudz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kbxyomhe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gatcqzll.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3aejgtinh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blftvwmx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hlneiprg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjqnqwby.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tdxmwbvk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ozoddihf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ocexaycx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3agcswlgn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oxamjlcm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3imybttjb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jbdbxujp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hdjhaeuo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3efcvaddp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bsmllrdt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lruafmdh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xltajvfz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3psvdkaqg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3drsmxish.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3londoohy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3csqsgztn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tsjinnzk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pcmnrzao.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kqjjjldl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xssnqiez.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zoebrlzo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bhfkvmsh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fnrndcjn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ugpbatvn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ejhdgydh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3vlxfaskj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qbnghwvm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3jwfbixwy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ijqmduew.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3clpkstce.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cifbgrgb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vfbbgttt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzwseydu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ddezdylk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lnswrlob.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lrsuumcf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3eljnbgdj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3etnmkyyg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejhfnpwv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qitmuaho.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ufjbgohg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3juwshjxr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bbawtsdv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wpezymtp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ueodjonz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gztkyuxq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wmqzmyro.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mxcqzmfk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fzhukzyq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3smxkquty.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ptshfqcv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3iczttghy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cyfwvbog.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3pyxyqtry.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ocawfaww.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hnbkopgo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pwnvdvhd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3huoysbsw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3npmwxpfc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dvedcrel.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3harngdat.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ooxaahwu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cqbkwnog.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ieirjsae.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whpjufdv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3febwapoo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ulfxtvhg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3niuwnlpq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oqnyjrgo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3usihiigl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pnrprhmh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mvodqsoj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3twcfgngt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zvgrgggm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zwjrmiat.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bycaxudv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mydfvxzv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qdzfmvkx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kohpkwrb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fbepoorn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ohmjyhim.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jenrospd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jkgunycm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3yhbluqeb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3afyyheub.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3plwfssrd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fbkshbeg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3mavkfrvx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kmipisqh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ogpbsuub.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vmwnmrzx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jqxdinck.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwbeiwrp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ywvshvqb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uvptnpvl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mmseqjra.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ymhjqbgg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dnyxyebr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3liwiuajl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3bohxmkcl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jpjjfnuy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kcroqjqq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wovljgyn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qmfbdchv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xszkpzdl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3paqnnhhz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vemihvcw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ppmegosk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnuuznrq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3yqgbrdks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyjkrpca.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pngfjsml.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rrcayubu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mecxhicj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cemqvimt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3skugxxwf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xerkvdre.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3skkkedkx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lawjcspq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vzfkacju.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jedopdkc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3mdszjpbl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3otzdpzbw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cslvmphc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dueedpwd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3msstkmwv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3chhdcwkg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dgbjpwcc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3btgfnouj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3uivyoced.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3geazpchl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3grmcejaj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3uxjbocai.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sugzlutg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nfycynxc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rkqsieay.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ydazgwkg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3stwekxfs.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dhpktqjj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3lnmaiiew.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bhqpviof.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uffxnixc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkygedvf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vfpmwwrt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3gztrbtrx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3uwwloonq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfqkbvgk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3xeqizoqk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3itdpssgz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3myvqatfs.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3avvotfup.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wzxflvkj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3iczkzqqv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wapslfek.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3voanbszg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cmclkloy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3mkpnblmd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3feedeyst.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dgrlqgci.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mkrmqbfe.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bjhavida.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3biumwhaw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nkykedil.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hkiszaky.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3divblczp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyujdezg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zzgptzpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtjvjyqu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zgwepkry.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3iupajfrh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wxjubvwl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xfhppczd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3faqfjmgp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ykezjmka.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xxhhaufe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tjhamyxs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qbuttcjs.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pivrlgyo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3apvqrmra.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wsdernrd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hhicocqb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wcodmkoj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xsdwpidd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wdvlxqbd.html


<!-- 参考信息 -->