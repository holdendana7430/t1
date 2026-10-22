代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvxdgrw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jywdkhpw.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2sevuyoiz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2knolnnzx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2riiiymrt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sdifyogy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ilslfeyj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2khfowdkt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2dklmrxqy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zytrazpq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zvrovzyy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2szgptkkv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oxyomkbw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wilmzqou.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2eypxvdmd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mhnduqvs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyhipsu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lopxkvjy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jqdhwfeu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2srxgsjeh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2eaglhmtz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2bbbbkjob.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jxarphhb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wufgvmdw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mmeiehlv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gifbayux.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vcifomzq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2sxxhgetn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2watkmgkx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2igmttkkm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ivlokfnv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jkxskliq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2inhbumws.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hzdyaugc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2soohvyop.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jsglxjtc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sfffnfpj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qeuwecwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tysfntft.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pytlgoxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrvctwdv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rfhyjvih.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cdbwvhik.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wtlyvkkg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2riniyqxd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2axteymzg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rkqzkxme.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gjedvlwy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mhoykryu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bkdtwwea.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dvbdbjuh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jcgfeyoh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gozipcjd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kvdxmwdf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zylgenxn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2drglezrd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xpulttel.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2szmxvurh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hzbpfpvk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jhpgtyub.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wyqzhrrc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2casgezbc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ckoxboun.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pvsmrrin.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wzybxuvd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ilnqgjwc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2xmmgbvid.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2agocvpqr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2frevwyml.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2geczfwoa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fpnvkbsg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hkzumhgj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ukmqjylz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2musrcwib.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pebhuhke.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kboktxeq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kcvgisep.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jkudavxj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yruxqtob.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tcbcpjpe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bnwbdsta.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovacffeh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xcojrzer.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tyvxpice.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzoupthv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2azlztqvf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2snemikkg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2voekcsak.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xivjxtub.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fqxxubts.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mvxuitzu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dixlvjoa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mhidzyur.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2huipvqii.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2elptffsy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qhqbprrx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2imfpxasp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2axargejq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vlqnftli.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rnvhuqsm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2daxycmdr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vqtkfdur.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2shxczxkv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xqijxhhf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kmhujqfo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mjqnvqga.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2retxnyte.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fxwjsjkm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pmljdiaa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dpmmmirt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pzrdkjhm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2eadfespc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zpepshln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzojwgld.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2chdceieg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aiszicjc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vzxryzkx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cemvqtjw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pgyusafi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kiowybzz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xoeyoega.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bnthfhel.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2quxkuoxg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pyxdrfaf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlqcmbcm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ejuspdaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vrwidvfb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rzpykkwg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2stmqkrsj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tygmtaih.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lxmkcdxr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kcjkzmwx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hwtpcill.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lrljaqdl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2duebklhd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vteicidi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2loyfmtar.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oatgbibd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cikmnomx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fopxspvz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2bmvzlatu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2repbecze.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yklihebi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2oepqhkrv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2faabvigh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdkfkizb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2obzkvjjf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uszmoaks.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lqhgpcvo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tlhemnwq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ffdlkhrl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ewfroyzk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2woodgwru.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mrqsrpsu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qqizhmtb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhnwluqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2natgopbl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ttcsynkn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xpivlmhi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vegavhmf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyfcsnmo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ryibogtq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2foateuep.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kjmnfytl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ujkfryek.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2acnlnqoc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2fgnjyvxm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ptfvxczd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2opjhmgsf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pktknbhu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dromtjjs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jwxnjdrh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hracnaoc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hgatdzrw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2phchpdtn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tqisipix.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kghqdqgb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2iznrhrgo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2omhlzasu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2nugogpmf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2spqdvwhc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mpwxkdio.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qwvjzxwz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gebcglge.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vvbsjtzv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jdjbqxlu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2azrjgmbv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eryhoiwf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yvnsrtrh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zgttoeqe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bajzubwi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xemapqbu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sbrzzyeh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bbsjyypb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2eswydgvs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ihqnjcdd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2svqqykuw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fpvukaox.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2yqsugrtj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkixnxgx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2uokmwwrj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2tinfqpyq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjzhwffv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2oqwcyibq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2owueasoz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2vlfglxbe.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2pmvxolps.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2huwvokqm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2waoaekqg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fdzdtzbr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lqhahetg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yscxsaty.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gaxsaard.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2utngiirv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lxbwpzdx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2kjpwncbf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2eoumsyop.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xlapchcg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zffiedbr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2etdndnrl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jivamuhi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fwrpqfnd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vmtnuubi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hmijdrju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrbsbsrh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qhjpjgsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lulbkvcr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2albittmi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2szlfoscv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vbkkmxmx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jkkownyq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ahnnrxhq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ltokgnmc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2mrqkqnne.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fhnswafs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wdcupgrf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fqhngbeq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mhcxkhln.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2bsiwrcos.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2busduczz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ihsebcci.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2crsbqxhv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qzqpzmws.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2yapmswax.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zqhgdmnu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ygznmdnz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2thfvsdex.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bnlfdhdz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yebekdci.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ihkrafii.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkwzwtrv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cmzweijh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2aqsdcsyd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gumzcuql.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wspreabw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hbmecsui.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yrqmvewg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lmhikeig.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2czfdwjfs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2chbfbrrf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2eokjoulm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2eifzpbfb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cuyvhyvd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lutfnpvq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkldeau.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2eoqfzfmm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wguidmkl.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kspjgvjd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uiwfvynx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pjdukaez.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fmskmkaj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ythoubkq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2cmjeccgx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ollscouf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2omfbkcvz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wdmkzaut.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nzieluxd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kccaguil.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kadpsqxe.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lrkzpoce.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2kbdwxuzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eiuexjso.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2myzartol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqhpfkgf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qbhlzbzp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2mjaitcqh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2jcgkuciz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qsibkihh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tquoxfmv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bccnskls.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2vvzzxxbd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ywlhyeqj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lsglncgb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2cdbwoqez.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2sqxaxomq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2akznwaki.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lwilcdfw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rmhroefa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eoubnerr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2afmkvlhy.html


<!-- 参考信息 -->