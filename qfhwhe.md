代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mbrqcdlp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2uenmfick.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gaoucksi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hlssrckt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gwizuslv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ybasuhgl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rztujnuy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cdmvgnqa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2bgmyjzhh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2agngujwe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2txzuqnvs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ntqfojvp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rtjofynm.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xxlzucks.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bryqdttr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bwmnyxqa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gyxrlcfh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyqkany.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xohbgfib.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ghopnizr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cwjkpnco.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2llojipce.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mpjlrqjq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ysuqhiud.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2aycdwigx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fpxyillj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dzferssw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2trybfttu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mvtroubf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mlaqiqsi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mmsokubr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kbqikjvj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ldutpfgd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hbkqowcx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2petvkfmq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wsuoqkhj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xagvjyig.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vszesnlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djyywwvz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zlcxzwlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewzoczfe.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwdjbziw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nfldiajb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2uivnkpbt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2croyfpif.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pagsmmvy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2akthwlne.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lfdojqwl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dudzwgkg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qiuvuhhz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dgrkjmar.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ckjjnruf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cdbatrdr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dswoezvv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rlrrxhuw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pmrvwohw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2chfooosv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pzuavoea.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jsfleyyn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tppbztop.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2crasgpzb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tbrjmaul.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2arubgdca.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2snjtxwqm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lzxnjlsh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vhzfktfa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vznofeyr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dhpuwoxr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2onxmbsca.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2czdiqdlb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2djzbqium.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rryzaesc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wmvhinsa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2jlmqooll.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bgpraxqa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2feuvoiir.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ejqanrbj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jffusdoy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pufgpewe.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tvofisqr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nyhtphlk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gpshhahc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqnvyjv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ndknflop.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2amomaggp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cozpkwgt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rkujhref.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pyyxmalh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bywjtlpq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qhiyqhja.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iifpmtze.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rjhyydaq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cspxzopr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2aywdmgmz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zzmkugdo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mbeivwkb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ajxfgbqi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ktnlusti.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sbzqhghg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kcgdljpw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2iytrodyb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ttiiwyum.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lhhicmov.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ayajwcxp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lfrswush.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ewwxopvb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ugzzcdfh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2htankjqm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uhpltvas.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ngjjmvgo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wvtkgqcs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2crbpamhw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hmzlgohr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcttriot.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lvvcjtvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezashkzk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ixpvdcmi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hclbsemw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qoyvgjre.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oukhgxlr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pyibubkl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fiyaznrh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2odazivcq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2bigdndjh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mariwynx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mfdsjzfp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qfsxdtwb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xawdaowt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ivsmkjkh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2idhbstqp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zsuuwbdj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfqlpgdo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ozywyrpo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ziuomiha.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2afhvyuvn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2uasdrugk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ojqibtlz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cjvilkdp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qdowvfpa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pyjrzsqe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2eiinlrjh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dkrvuosd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2pqmhtanh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lfzqwulx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbwncyca.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcbvmlgp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vhsnxehm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2blosvzam.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oqyvwfxo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2imogawvd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yhjztpyz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vpftffbs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wqysslvw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qouogwut.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2nucefkkw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbovxort.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2oujstzil.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rxczyedp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lvqgoeld.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2sqssrako.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2cylsottp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ydscvakv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iyrfubgk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2khaqhnfc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xgzukmck.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wbcphasq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2mnpjmaaf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pocbikpj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cirmdjfh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2osoiktcd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dnoeavuz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pdigotko.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lxwoedys.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2swwyxgne.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xrobtlix.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cztuiyqs.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2scyuwnnq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2afcfvmxu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2sqyuzjxg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cbguuyve.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjedxby.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mkaibmge.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lczwcywc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lzvfklrf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sntslkfl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bhhinguw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qmwfqhec.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oflvzpwk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2prxadqne.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wauknmyl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qyxnwgdv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2futdtatn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2bmvppvxd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sbmhzynw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2grzbnsmq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ktpeoopv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jvzneypb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zhwwcvpd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2turfyoyf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkskxuje.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wsrffgnz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wcdygkaf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gtqjdhia.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2saspzgdl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hmxhsujf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aremyiuq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2royyosxr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ctdahros.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2qedgvzjo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2osdrxjth.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kjwnwufq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2smbzblqy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hzmotxgp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rsidzvjc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xxvtytwp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jsvifpok.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tydpncmf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vqszkbzc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2grhoaedr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rqzcntvg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rcjspjop.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ptyddnrg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zvyvbglx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bknomssa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymgcfsnj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zpevgqqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjyhlixa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2iqfqbxpu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2uvroseqf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jgrgvwrs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wxqwniqf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ozuokmho.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jglybybi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jcinhrvo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2foxtqqze.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2sawyrlsy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eusjqbzt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2arybzmqa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2aqjdeygt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2unevcqay.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ijaclnyn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yohvxajp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ezxvmtan.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vxynwlsk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rbpfiqas.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2cexnxqtv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2muxyjsez.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pyhjbywd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2virgdgob.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hawwffyz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2smlrgtbb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zunelxwk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xctgbayy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hbcxrxjb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2flqbfdel.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2igvuwumw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lbmaiedq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuvamvla.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szotihec.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ryiksqcd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2yxvgjevu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2mqwrvdwi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sypreeqp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lbxebjmi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ocmblxux.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hsmezwpg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hauvswix.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hjvoubgy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jjoitghv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2oybpqzlm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2afwmztzj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2omkeprzd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2yjhqbntg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pkiikmtv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vkfxmpyk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ekejrypb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fsczmgce.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2piekdcsm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qdtosiie.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2omtturci.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2scxmeqtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewlevsgd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2hkrugupf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfxmbozy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zorlhwyj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wvzorzlp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tvmuqtzm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pzydpoku.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ldigxxwy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2utexovjx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lbhhhtoe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mruwwerd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tuiohsko.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gnowgjcp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rybzdwdg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2asvvgqli.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2phufrtak.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gzeoxoyj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hzosuhsv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ggczgigr.html


<!-- 参考信息 -->