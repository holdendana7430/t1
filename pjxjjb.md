代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bwgtubsz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zyozohju.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qqtteqyq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3zpsowwus.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wpgymybt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xlehblce.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bnbeabjm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3yribtbsq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3pzwbnivi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3puslyggb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jscilnro.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3shgwsehs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxroqsqz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nqvcxwim.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gwanbqpj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pskzmyaq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3utdppmwu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3aasakwef.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zfpelmle.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lsvwcjqu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gtjkwvhe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bamohdhd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3cydjnvik.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tvtumtwm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fohcsnch.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3pyosjaus.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3oapzygph.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rmvneslx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eptgjsxn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3loggrbhs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3upuoygsl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3hogcihil.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3evosqiyp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jmynxarq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ukfgwfcx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3diieskhv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3thsnrgrr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3idqqgvfy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3safgugha.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ljsopuvp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zwkephpq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uqpppqkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsnofpbe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nnpyjorv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjwtdlik.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3idjvbgmb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mnnlmtmc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fvqpnvmx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qmgyehsc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vajkqlrj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pyhzqnzx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ydxgryjd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ndairdvt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vswgnvtf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ikacxkap.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bqkfvkvp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qnztjapp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dopuxwfs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rarvczgd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ibxzdvoh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gztpfpkr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mjtxozkv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3odfsssit.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rcfkuwgy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mhhofilw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3btqhgesd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rmqqpnlx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nzzgcmns.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3aeimdbbt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ycigtnaf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uolldhzu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cmzohlnd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3egtldsoz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ncjpwwci.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3iwhvpzbz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pwxujluw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tirrcxsn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zwvbmujl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wstcyude.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fmipqpdt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jmhkfgwl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xtjxinpl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qypuayws.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fuxbrghi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvxildq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dcwpuadr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3phubcmxm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xmjpihrx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3temvmixq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tuliqxln.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rtwfhuyn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kvtvklzz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cxmpgams.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pvektfnq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nvbavccz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jfnqxmcq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3oojtgdux.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nexfigwm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3njrzzpbc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dwemtzrq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3otategby.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kdnnwvzy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nlmiazfp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wtcwqbya.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3meotelup.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3spmvucxi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3axouytxn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qbejyely.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3becpcfxg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wqarmqmq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zhfjjwzd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nyualnrc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xxdnwgbh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3uyijohmq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3gqafqdys.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pfhfrerp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3omfuhwox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxxolicy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jmcneaox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omiroebv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xpzzkjah.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nhjoqtej.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3plugikwq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bgaiodgc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yzuqwdor.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wolayixu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3txwwhrib.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tryecqub.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zsodugan.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3alsmgyck.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3burtuqiy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hnjkznnf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fknuzvwh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3naqeahqn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qfqfygkn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3toprynfk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qmfmlxro.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dxogolrw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3fbxnuatv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gmpqucrc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3oxrgyrdy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vpxlfcql.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xrlotatv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jdmvdyrh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zcqzdtuq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3joejmddx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wrcehzml.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rjojxaci.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3arhitmov.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qulzerux.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dlmezhfc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vhhxgzit.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yinzmfev.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wubsimow.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lahopcck.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xldiabtt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ziyeeljl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ufiqjtyc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wblepxey.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wetgzrrm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zieuhmzl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qxaouavt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3usplkqtr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzxmwfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfcfbvyl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehogyezv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qezzdbnn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xkibzobi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gdhiqdnh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3etnwkthy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nuooixye.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3woriotss.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3njngartr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jnqoxymd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ofkltord.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dsmahaab.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3werbtljf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ecfsqbdl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xwxhcjaa.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3gxlcdrvq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nkdoxszz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jtahqkkg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ixluxsfw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3kbhmyjvr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wowgpkfr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ynlmtmfz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3stzhrpxr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bimjhrdu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ixaphezz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gqgcihgm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qiozdsfg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3catakgyz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ykpnmyxa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qhxywgoz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cmsbcbdv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yetcxabe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ienxqjco.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eynqejgm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ldumkxae.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdwrxvtc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jkjloicq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3utzrpleg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3skujtaha.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzfupwte.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yntfmqrj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vxhndxji.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xnbryhao.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3eokqvcmw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jswfiusi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3uxcajmaq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3iebprhqi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hblswlfs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vygpcpib.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gbssbriv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tjywjxoz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3twgqocbr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kzrfotiw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dtrxvmio.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3srmsziin.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xsuvnpda.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mpdgmswd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nitdgzgc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qghrolmi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mssctcgc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3reazlnhf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tgtvitpk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xjiiefwe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wusqyopx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsyueecn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3iqlrzent.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkoekqmo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jwbketbj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wpojuotu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fxvxcqwl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dlyafecy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ixcgbxqm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ipgewnsx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3kqmeuwks.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3inlnixky.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vqkbviqf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3etklcvzm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nizhakbo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3wnxrsyqs.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jossbttx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wkkcxqzu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3izxjldqx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pnofspnv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3iyrfksox.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3fbrezkoc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vveyqknx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3urknkxai.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jkmjisdr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jupkmijj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3epvwtnxw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3acogkche.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wbmxkzlb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ekqzaego.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xbnrgavc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ppxnajqb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kutpilww.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3rnhyccvn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aznfnluw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3srhqyzbc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kyqmihqf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3toxwuosd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fmwknaam.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vfqlgxtb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fcddwdoy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ymgsuqgu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3nrsaoyft.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bmxovrvp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qoxnjxji.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rzgtgpnd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hquuwgyw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aclehxpx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzckpgub.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xbwyeabf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dbgffrvz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xklldapr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ibevelsv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3gmwvvaww.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uacncnaj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xsdndems.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3moveqyam.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3rbzrlcbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgfzwxvf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rwpmwoxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlymhilp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cjizcmti.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fsfdhbfq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kjjvpyrc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rnpvmvwv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qczezzhf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3njjqgmpg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uvvrqmly.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kjmyvfva.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cijwafox.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3dmnahpdw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3zarkktfg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxynxgka.html


<!-- 参考信息 -->