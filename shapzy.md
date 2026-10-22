代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ztlafcyr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2sobjwmrf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dmtaennh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tqqkjemk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dpztzvpg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jjewxkic.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hpqtxglc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2aupawikj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ulgnaama.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nmalpnjp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ltodsger.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nbrckoxv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2insvizuy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bqxrimyw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ysbnurin.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xglowcqq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fipuzboi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xrmqjivz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2uczffyfl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2heazlvsk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2znnshrkd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ktcjmloa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qtiongzr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vrioinln.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vqlwxoob.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2smyczdjb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2blwmtybt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ireunzep.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xttrqefg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fayoegxq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2inocuosu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ftdagqvl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qqozjmdo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dornbzot.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2umwedsey.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tkdxbjbw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bbsnzwsr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2odwpnvkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agpydkcw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ccgiiicj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvkqwpmd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sqotqiga.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2aizhfloy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tzeebjoc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwlcsfj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vtewbmyq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xgdqzgio.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ltyvhvht.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rtvfjlad.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gyowgiac.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wxrulubh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ejywkpng.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hajqfkyk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bybxgkgo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2exlmxofo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2retlofgm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tuphijxk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jwehzflo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tslftiwc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zswuqcls.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jxzquupv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hbakbuqw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oekqodsz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ngggnwxo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2izsbfxwm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fhsbjsbd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gzzzpkzc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ynxncdzo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ezfezddc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kksgzjen.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zyvfsubb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cdcokxts.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qhbzdzxf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2tjapghaw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ogeqxkhi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kgtovudw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jhrglxxk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zptlvrbh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwhrvwsg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kzkfcxgm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yxafural.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ngsfaqej.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdgfmkvt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2obiatjll.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzbnrnri.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jzntlske.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xknnbzcv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpdppouq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2inqitilw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tvzrndua.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xtsewjvl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nalqgzve.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iyidfevo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mtilbujb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qqlghumv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fzmsvpdb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2adzlnznx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2etjiihei.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bkhykaht.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tyunkshq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vwlqshxf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ypsufrli.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2aghaxpmp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hbdckhws.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xmtdpdpj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rbkjcrcf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vtvzkgrf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pmvecepd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gehpxqbe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vcfqedpk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ktoemrlg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ehhzxlzx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jpqtcfhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuncfxqg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nwxgnpaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymwczfsi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jwflqeul.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmfdigjj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ltdbplkc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sxlcsuhh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jithkxbi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2okmgmcmt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgqsocfr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hgaefgmk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgathumj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2suegsski.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bjzsayvp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cwuhhomv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zmersiaq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tpecpwdi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rtulpgcs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ymjyovft.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vitegdte.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ibkyhavh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vceprmoa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ohjfzrgw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2phxqlqkk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cajivknf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mktvderw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ngiuvfmz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2agzprhlo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2kxpanchb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gnytrwuo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2grnczcvk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kaigeuhu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qolzhplt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2codcnnbo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2thlnrkcs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2aubkgcwn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bduodyzm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ntywezra.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2brtxeilv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2adgqwtyz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xgvscjjp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2amxokknd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrimfzih.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vlqwwdaa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jzzbxfwz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2agvzxbbb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xkijmdly.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gffryrhr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zvqmlgdc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rxgepauk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fphcujlu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fnuhvbze.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xhucwbdt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ymbtulnw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tdhdoyug.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ewhwoesf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2svjyepra.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fitiuhqi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ftfdyzzl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2coixpkkj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ywjuvwja.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jeyidnql.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zlagkbfc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qivpxaed.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2petdorzz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2uctbffbd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xoaldeqj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2subnxncg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qalciuyj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tfhzenns.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fhlvhhwg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kkbtcsgc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqyhbuev.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rmjwsjnx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gfexrdqu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2axzqrrve.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jivvlkoa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2clhjonmj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nwqfgzml.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fubprnxm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lpdtgqoi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qtmnizdy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jvokltzz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hfemsgrv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bikodnyk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mciwbesf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2kebdeksk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vkzutocp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ywkdwlnt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fskawimx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gxrqjzqw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2krdtusur.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgemxjem.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cewveuro.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2bkbyxocx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjkkebdh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aeyimxak.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pwsyoarb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lwaevtjy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gokmhgbf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ordvbssz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gkxbnftv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2eizeuuqd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nabwidsb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bugqusgl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kwqcxvmd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yqcawohq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nymwhfef.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yrquyixc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zrnraupu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ywclfwbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uefrlujt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2imhvmmaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfowjemj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ucciyfgf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2umzchano.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2oxujboec.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zhmzfqiv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2njdrdltz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kyfqlfby.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bglgsbaz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2giytoqff.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kyuwgmhr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2socorfmt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2zgraxihd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2lqmxmltc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xzjfmvjl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dfkcwikn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkdbnpd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2opmivgtx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2drkaowkk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pwttqqsh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2kwlqsnwf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2sbupezvs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kfxwfaia.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2lnyzphgj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nrwqssgr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjkcwcaz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2kcjbftyb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2depjizle.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fzunjexs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2emmynxoc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xzvxeqzo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2juqonvmw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukwvdlph.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqxlgsss.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jhmbgwsj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hqunfwen.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2lpswtsts.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2twszhzod.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kddpjycg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xkrnjcwh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mzwtzrbn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2roruenzo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2erdgivjr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yevpzmvi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jttbubdk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tfwvulia.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtjvyvp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rnoicbwq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hpxjpunq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wdwwjwud.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2agpijgsy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2twhnjylz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wmeymirh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wadsxffn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zbxoqthh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vedioecb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntlpcicw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2lebfmlbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mspbggzs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bogkfwfz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gmlwwnjt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ekfmzrvl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lzueihgs.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cnnhxjzw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2vmimxdtj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ofqqiarh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vzhagobj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hewmgagm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nciyetju.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uhfnnxjp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zzziplmj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qdthdqjc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rwswkshw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dozzgprt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2gasfrobq.html


<!-- 参考信息 -->