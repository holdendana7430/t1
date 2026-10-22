代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2brrpssvk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rrivmpsv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mvheofpm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kqhrsyvw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jbfdvyrj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ojkczwbc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2kotypyhc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2efsozzia.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yxkoazqs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2njuhqbpp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jphmwylv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2btgffqnk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlwioibv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wpcyicho.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2egaasowj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lppokgpk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2voqhpkop.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kofjsgnu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vfgutnic.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gikbnpyo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2svxhbcpl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jhgibayw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2oqdfkvdy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ksxwfpin.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qakmslnm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qkdbqcpc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2trwpigdn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lopdrnji.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nipbjkuq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kcsvoehy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tzlzqvxu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hidjpjpf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ztcniclf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2oximyhcd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2yoihdvwb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yequnfkm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fmsrusrf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ufrqvdja.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wougkjed.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jiottxei.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jsqyvjun.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yfyfvbto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euxojtvj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xeovlsxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuzwfsvp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mgblazaw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ljeygntg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lmwpkxti.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gfeiywbh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2csystxhs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bjfkkwve.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zezmhcnl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ymxtsuke.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vfqwadkg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yxcyajnd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fmwjljhk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jygppdlg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ingovlhu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2orpljzqo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xknhlwhz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xizuhqwm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2reentcea.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cigxmxsf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ruglbjrr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2havjjooy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ohfxgbio.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jclxzcvt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qxcmdquf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fccxxnjx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mwqmhiej.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jprwfvuh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dqiclzja.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mqgnzyvd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fzaqysbp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ddyafcnv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pzzkaihe.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xmhpcjye.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nsitqumg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lvczhmua.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vuyqdmgm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2viaspctq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hhtexgmp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uauritdq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ehxgllzo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jlolohgk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgbswlqo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vfhnoatf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xaftlobi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2leavtlug.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lloulkmc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cfpblecq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jbipqnob.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nzljxrem.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2idtvbgma.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vaoyhbxq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yedirifh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2brkalnjm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zbzgxtoe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2smlsyuql.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2imhzrdfj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cmpxzete.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uzhdulgj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jjzwgmhn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sbeuqcqh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mirxxnhh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pocmtinb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2flfvjouf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vcbgcfnw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2dvzczyqp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dnajjkzq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ozocrwol.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vlyvpzqz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ghelfcew.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pzlmlnro.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gvyyikjq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ktjhipix.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2agihreek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mailmtqq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mitneqgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buslkqwl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zchpcddr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2drapuram.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ngnglfyv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qsrwgmtp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wwxemqic.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kfjxvztx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlwgjwci.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dnfstfcs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2layccxev.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2utvzfdvv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dcenybul.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2prfoknna.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rjywvzct.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wjoqjooc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yjrvraod.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xcyuezgv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xmliwnzw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ctpeyyug.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2krnudeei.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gzkglcvo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ubwhmvtv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ylkcsihd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xbwbbmlf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2etmazokc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jihwwjpd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yywwnjey.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ezefxxxy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ncakxuwf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wpmpmfgk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nssyvkaf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ryomcubl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ytqqgifz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkwgekmo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vcysfivx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lyndctwx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fewkougf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2poivavdo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2menxkdme.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2roqnkzba.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2merrflbm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2iktdwnng.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hubsoqzx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jucjyvhf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cpjcklsr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzjfvqx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yyfaqxro.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jqgdbxyc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2atrwhfgc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qhyauvjc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yncfmdem.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2udebotvb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fekvcubi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bwtakxmk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ioqykdzg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nhcashqv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gsdzdbpn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2igqwkmyo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mylueaqm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ryyrjtbk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2homxuxku.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ehllkesh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ocfyjxwn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2igzxtofn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2npmzwzbk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ivkjfcjw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ltbljijk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uqolbcoj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vqgyqzjy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gsjcgbtw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2skhxbgbs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xsykehvd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yrrlttvj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qoroqudz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ygafddap.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xgxxfgcv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ywfglbzu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pffidheb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzfxjgvh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hzmoqvse.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2watqvnrt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ufyuphwe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2pdisuxjw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2jyzqucoh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dsetwryt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qolvxrga.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zpjrulgk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygnosnrn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wijbtqcy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2cbbwxrxg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kawklmid.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yqhkrtey.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qgsnswlt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fxehalko.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jqrxtuor.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sdonnapf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jziqlwjd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jkgwehbe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2odltgukh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kgkbjulh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mjmazhjf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ccmlyjmr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xyaugfsy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hnwiorbz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wszzqxho.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2lmqwuzji.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kxyydmrw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xgctdosw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sxaplrnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulyzabid.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2yqhxotgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jypeyhra.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gjquixxi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xjifozgl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xwibckho.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2zrwrsfyl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fvdspvwq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cesqjsrr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cxfkocfs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zelenwnq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lsytsprb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ytmybqkm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2szukkikn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ognzypls.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ezpghcrs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hcslzmmm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2yupdwjge.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2teyylxms.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mfphqwtv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zknwcxlc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2fhhwkaln.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lxdijftb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jpeeaavn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kiscxzls.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gvppoowh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlqkuqty.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hlvenxnf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2igvbyzix.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gctdkozh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ozksfxjh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rymsdzjq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2uuvjdejz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cubcybfk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2llzndijj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hrugguop.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qqkietbf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fkkqjwgd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2sqkzljwe.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2delwupgt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2sptrapms.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gftoccxn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vaomxwgd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cczormrg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uoyiqlsa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jbderfgq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dfunaebf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2jejcbaoj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ycppqrsp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2npalvaip.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ezvkqoxd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lzbfqbbj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aqkqrmbf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wgywrwqb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xreymuci.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ymtetozn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vtnezvbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfndrcck.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfbaiubj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eswvdzgi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bclradkv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2hyhihcvw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2reizysiy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2aetoywgv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pxkxntxl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nzwgiban.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2snevcvry.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ewifwsbf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kzmfourk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nryeqinr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yentgqhp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbfqkhnb.html


<!-- 参考信息 -->