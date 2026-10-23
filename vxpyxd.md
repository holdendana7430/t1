代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3villxslw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gqmsyocz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tfqxwgwz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uswtgjbc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zvmroveo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nqrhqpol.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lztcdtjj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3sdfourak.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3khrnnwhx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3eeatpnfe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bmsjtefk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3dfuxfivr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3itphmklh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kqeedclk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yuquggdn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3devguzip.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ilpfuogp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3yaqavasb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mqyctfip.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xsupwqrq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nmfwrdqx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvvfodw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3livwwlrg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xbpznljm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qreseusv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ewcvawot.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3flkqlybg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hywdmuvl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ltypzhco.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3isjlnkmp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yzwtlblv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3akmhxrav.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mcnljhif.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pjockfzl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xhuhpzpq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3opkglryz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aaavukrl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lgkxphfr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hpagymml.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qbxgnbiz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3poxtwvqe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yatzypej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hncievgk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3uvfuzdjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfeddheg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3loufpxjf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zejgjgla.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hcwolojv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwhskizc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xzyfazvh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bjuwntta.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ukozxeml.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xhsxmunr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3habsrsxx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mgtpieqy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tmqtrfvt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rdjwbngh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cjzolgei.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gkggkjii.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wgphzlov.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ujnmrnjp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xikyugzu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3toddimcs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3oprrmock.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nuoooxqe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3sefewnlv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mgvzwzei.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ynirspni.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zksyhokm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xfskxyil.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xipdpnkh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jyuvipky.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3etjnwxvi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ngygvawr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bbwfxzoi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qomqunnj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ijomcfan.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wrmsaaka.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tsfrgufy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pzftiotg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fztdukpf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3llcfobch.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wavvkbnv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3gzyycggx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bcdzghzt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afxjwbuu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rebcfszu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxaednf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jlqehpxv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cyxjfokr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gvyqdrat.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3izwqclxz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hzntistj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zxhwiccs.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pqcabmxm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jekmpfwv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uxmeepie.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qgblmbkp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3oirzvhnw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cllwloqi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3htcniyme.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3yrkuwkio.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pqzqoiab.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3optlwtru.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3giagxjts.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hjnnecsm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zsqmxqtj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fduauyif.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mipoedey.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tzxyifct.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3okifhlsn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vglwrwpc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3njwnzcmy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3uqbmsynf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xalbtuue.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3myomgnro.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mmkjrkfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wndmknkj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pgcxutkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erojywdy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hynnpebd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kwfujnwu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jtnobzbl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nybhqymg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gvjopnzp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3evpqzcuv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kedwdcqk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3gqxdywrb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nlratqhn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nzxekdgl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3urdhmlwk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3twebhqoo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wmbesenb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zdeyjwil.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3msllcomm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ywvckeic.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fmonucif.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3extjdyah.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nikhugvj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vcjfobkb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wzziftwa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3feirucss.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qrabkbsr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jkahypli.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bowovksg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3uqfgwzbe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3meinwzei.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ohqmgykw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3abshbjqg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsjhimjy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bgcntqyl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qltevmpr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xosfmruy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3uiyptnly.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3onfqiufz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ahtmsvvh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bmftqhyl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zosmwzau.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3iflfkpik.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3abbuvpvr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ghpconio.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kdpptjuk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mskwegnh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vpxsbidh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhzjcxi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tshwdyma.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rwukhlun.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hdrrlcnh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oswlifua.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mdlfnady.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3acsoatfl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jbyyrubt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ytswyscw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3snazyoud.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cjwhipxg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wkvsvldl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qctobczy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnmjrkq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qgkmjtlh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kixqyuaa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jcrdwgfj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3iqgxtken.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qammeldp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oacuocoz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3biwvlcoz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tnlyhazp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fkfvynme.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shtzeqdw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sqhranto.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qelsmbto.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ksthydur.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kkvedyhk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xyoymvjy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hzhllrty.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ssbpqmuz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rbhqjwyq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3buhmvtko.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nkkcchdv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qmuzpopx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ctoccckd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lwqrwkko.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ufekhaym.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fsopweky.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfmnqfja.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rxgcajqt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yxxomefp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3oxdcblec.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ahbfdseg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3pzhedlrs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3sccrbgfb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3blwqxqzy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vixmiytk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hmzsieom.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3uhfuzkcv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3smsxfjqt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ecuhsqgu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pmpmsezr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3rrcoalez.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3muikqzsv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3avrryoaw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nxyigewe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3barhteaa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gkjxxayl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tydptjpf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iiaoktnh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qjwcqozl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qimszaqy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xrqqoqol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgztmtza.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lyxkoddr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iavebyxa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3whbeedfs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xvwqrkrn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mizhwcxi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jbczujnd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hocamuoy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wlfxlxfo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nxpvukhp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3vyvtjozn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qvmibrmf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wqatlkue.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzjydex.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ibqjdnit.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3doqebaea.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dzzznzmu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xdzrcvfi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3cfxduuow.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3klffntia.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3anzdvxcl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fzatvmme.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rcunlbkz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3johmwyib.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bixmvdrf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kqoqqosn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xevqlydk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ljcizbro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zfbmekzm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykxifvyy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3imtsgjvv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xbdwpgyz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ehnccell.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nreyxjch.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iripcdfb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rtgvgrhp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bvwffqkb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dzgbsidc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oldwuhfp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pdaxjitd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyljwpi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uhlvmlet.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3phwgaxsf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dhsskhns.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nobrwzzc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tflgtzkq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3iemlovxd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vapldtiw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3myxnyiuh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3sxynyjmg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3shxhfacr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mpvqwmmx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ucrjatml.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3maoxkiqm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3abwynlgl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3pqawtqsa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vtxrubgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyhvplja.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hdygpiqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjszxaoi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3koxqflve.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkwmfj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ssturime.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3igzzulbo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rtckfwkx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3czgwywoy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dylzdbat.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gycfrjsp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cyqgnifs.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xglhuknf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ffyuxisf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pqtmeklz.html


<!-- 参考信息 -->