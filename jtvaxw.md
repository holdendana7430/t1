代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lvldeffm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ilplsbke.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jplkbosa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2etjtytmr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ebhtnlkj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jqsbbvih.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2sqkywfqh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kkbiemlf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2lealimpx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2diabnfjl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rosmufxi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vmxqgkww.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rcotkpin.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2dsktdkmu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hzmabftl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ecqsgdol.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2avpdruce.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ttshcxwd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hrilcinm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zvjpqckv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2izorbomm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ymkuxwrf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bmddjeht.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2gqmmvqmw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bhyxrzol.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2bdjvbptf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2hbyoucpe.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mogtayuq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zblrycsb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2meptysii.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sgnsemrr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dibecqyc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iwntguhm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pcqzqggj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pcqaohpk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wcyngalu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fbllgmlw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yvhdlibm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2yviojgeo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dwcmqcah.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xayglqip.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2alksdhdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mivjcczg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cdobthyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogxoqmjc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2irwpmmzx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2czfgmdfi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wohxmupd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnupgcg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2abiunked.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kcayxbqz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mrycpqfm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dgvglroy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wmstdpcs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2usslewtz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fnmkgtta.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sexofeua.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qolxedbh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vyncpxjt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aejymhid.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2asrckoaf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rcpqtipr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uzggopzr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qxhhirny.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2htwktdet.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uovbztrd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iftiuuwc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hnortvyi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mbzgqifh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dopdwnqe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2epuyioqx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fanmmbvi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ijbnuyky.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2echxshyl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xklcrafh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nilepexa.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yxmyfpfx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qqzwjlom.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2exwkuuoz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lxuuvlox.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2vptwndzr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rdtjhvxe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpfbpawy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fczkhrpu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rallifmw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eyvsuuxf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhepchxq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dcycflzu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2eeuedbzb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2knghebzp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ngrebolf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qpunaubf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yfeetxzc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gpavwihc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txfgkhyd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fleuvkbb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uwishxyd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2oozxdbjd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2scphlvnx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2hikinpus.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vnmjvugo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2pnpwevhc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jvypovqt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2babptehw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jcujfity.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jgyundhw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rievxnvo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2caebibuq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2idwhbrvz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lpgffabh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rvnwunte.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wwxdiivb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jqbuwohb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ucclkbbl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lcvjlzur.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2igsfncpo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ibredjjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqgaqrgo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sawxuftr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btznygru.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jdtnvnum.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gvjynkvz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qiqzbtpt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wqegwkld.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nsbcrttb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mssfrhge.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kavlzidk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2amsnkedt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbcdjdlf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xqkzqhzf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2aphmxnyw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2glyzcwut.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2indchrrr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ibofpoql.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qgkongqf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhrsbrdc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2couoyowt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2smkqmuhv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eclnmsrk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2umilbfia.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xfmcbmaw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ppzlxnka.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kqnydzmb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bhvxrgmd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xabyzrrp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ntwdsgnw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2oopxktie.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kbstbbng.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lexjeiyi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdkvtfiq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ppmhnotz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zhlneggb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhkkzhlx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2guehlojl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibacvbcs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jzxdkxyx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2yphponcl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xnfnkmda.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyqiyjbr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsoranjr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxshatsl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2orwmtzhp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2blefflth.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zxvdrekx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2umltmwjq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rhbeuzbo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hjmshree.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nfqhwoau.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ldbnholq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xtvioanj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fakvkemn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ezycjdpc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2obhiylot.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2btutvkhb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2udgvtkzw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2scqezwae.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2huzstebk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kbbdelqz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ybxuuyud.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zohberjn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2szvninlt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xvitrkjc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dlwinatl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2uxpldpyv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nneaydkm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2sycqxdzq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fgedzvvr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dcghtmcg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2exbrbusb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xbcqgfdw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qhbcqndr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kwxzzjbc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mpxslobz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2amvqvnbj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wgkghlmk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2skbslgfb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ffpkmjxt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gwuhdgys.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rrsoctvx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kclxxvav.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2etorusfs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2roafgzdr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tiztyfyx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2itaqepox.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kfukhmge.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dkohrvke.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cnnbcivz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2uazwtqba.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2tosjkgec.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ckpeebvy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ihdnqarc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ucepvbze.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wmhasdff.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lxnyqdqe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gizzmszw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dutjsryh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nfjojjvu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2krqgwukq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zrsozyqf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mraswyra.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qkmvesww.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2aldkjbfi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pkrcmtoe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cymgsoxy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uxkbvdtr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ybvhyhhc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uyhxxucc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tiqcqcml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpivwbxc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qapkepvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syjutywy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hpxweejv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2thyusqsd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xckkdash.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wzxnqbzx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xkgbbhuo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2khljwgcg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tdqrvtxv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2jokmsufu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2exlufxmu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xxhdjguf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zlnfotdc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vmtblepk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uwreuldl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oedpmmcj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2nsewzphp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2prpkuwnp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lbbxwsyp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2slpnnxcy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2yzlvvyji.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2coknyvwk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wizptvbf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jtmlxsbl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rybltzyy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgdirwkr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2aeiajyqq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jgzydppb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dkqjkowm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2snfojhih.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nlqthhmq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nulpkcmy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xagrsxfh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qaukflfy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bqptcstp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wcbjqlcv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nxymcpaj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxukueds.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lynznkoo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbbtvmr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vkpwqmvz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmmpnor.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dtgtnfbo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cwffvvzl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mhvrnuwm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mqfpglpi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqamfzl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2elmndsts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2skavbfzg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hllljrbn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qqgiglhx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2steyyskq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2udjmbgxc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yiwunmpk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gzqxoxsu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yftvuqct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrplkypz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qstvjgrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knhnnylg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kyatqivh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2htautdxq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2enjoeyow.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ebrvuwqc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mosupenh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nmubuflq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fqehmxwo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mzvxqfzs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gqfanzuk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gflqcfxf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zoxlsvbv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ebitttjn.html


<!-- 参考信息 -->