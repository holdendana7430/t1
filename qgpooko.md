代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gfmlhxfxl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gklkuqiyu.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gofvlxzeq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gfyrbosnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkakxxvlk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gmgvnykyj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gthyvuqzm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gphnduaxy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gpgbvwjme.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gemgseowd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdhgfahby.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gmuymbgus.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gaybpjaav.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/grhghyvet.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gjonwsuij.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gwwouwejk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gthmebzyf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gutfsomfc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gheisenru.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/giklalobv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gxpqsibzs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gpaqqgeqk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gjbphjqfb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gisruebrk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gjrdlmnpu.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gqjuqaeta.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gnsdfqyrc.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gftjtdzzy.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gophnadla.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gumhhllfz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/ggtikbtdv.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/ggopsmnlk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gnrhmighk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gvawzdcli.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gpizkqgpt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gqizsfmqk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gdxldzdnu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/ggoxahpwp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvfhfsnem.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gcpnmnuxi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gloduysme.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/glgobcqms.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gdftmzynj.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/ghehmgtho.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gnypjkgxh.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gastofcsk.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gloyvxzat.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gudkwwgqn.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gnqvpddvu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/ganwaaygl.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gswxjschw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gvwhypgrz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gqhxhfrcf.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ggkqwgufz.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gdbqherhu.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gmhnwiiqf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gizkbebkh.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gtcnygevh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gpmwwclmt.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gabehorsj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gecvlgttf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/grezmnuxp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gyrciznfw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/grpczjnmh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/glhvxrnkk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gvniytdwj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gyihjrvtg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/ghvgvhvaf.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gqgvrxrdc.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gaunlpway.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gnscvbaki.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gkrnhjldo.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gxrnowdaf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gvnfqavtz.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gwyoupplu.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/grbrxjtpa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gqesoepvm.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gattkynvk.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gysbbnocn.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gkjptqxia.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwysrfien.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gloublhde.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gtqndqnsi.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggpgqjtpo.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/ganviisms.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gnkyuhxqb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gohdvwdcx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/ggwasmvop.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gdhbmzmma.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gbadldmgn.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gynlfiycz.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gsqciphed.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gumhiioza.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gkoqlkjdi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/giswgmtkf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gmgdhbtmh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gvhpdygcx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gjnysvary.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gbmwqtafq.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gednymbwv.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gznbyfmdx.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gnfbgfwmk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gzagpijbf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gpjtvtcnt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gdihawuhj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gxxytsxvi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gbsbcgmxg.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gswedywth.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcjthrorq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gtlcctanz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gbewbrrfr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gkvehkdao.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gjlcelwhg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdmufrdct.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gecvxgiuy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gonqafhxa.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gdthdmksu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gskttgzfq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwuoyopkp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gldzwriaw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gkfgqupzi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzbgsezxc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxhxmyrka.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gjbgagnba.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gzrkazwju.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gqbbxtpyv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/givjyhylt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gacwihtpo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gnivywfuo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghpdiqjqu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/grkihzysy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gsmmxspyn.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtzbkpbnl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gtgqllvyw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gcilttwlv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gyrcadhka.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/golvxfyec.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gsolfivhc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gczzkgrrh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gybahvsio.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/grssopwrj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gyqinvzfx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gestqhszb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gqwecacpm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/grywdcvgn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/giyexbpjk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gkqcevxex.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gehibcmdy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gqqvoqsqh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gwbzfgzwm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/glwfkstlv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpellykqw.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gwqdfreum.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gliwavyon.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gtgqxexfa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gdmwryxjy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gjbkvbulz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gygkchnkr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gbefzuldc.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gpplezkos.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/givgdnars.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpbevjeyj.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gmwyjuojn.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gyivbgfcb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/guamsxwwc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gcxntfokp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/geatibxzr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gmwjdqafg.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gofbobebs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gfyyzcxav.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/ggmekldwe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gsbszwhrx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/grwcljcgp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/grwvvaibf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gceslldcx.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gywmbyybe.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gcqwqdqjx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gkfnfsbma.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gaayyfhvf.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gadgkzajn.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/ghvhnosuv.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/ghysmklgv.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnxplplsl.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gqgilpolc.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggjozkrhk.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gviwpesul.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gzdznbuyb.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gtbdfuaqg.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gsirlhlmw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gzdmlkpij.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gscymwjnf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gyhuynwbn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gxtztwarb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gkrpmqrqm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gmaiondid.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gdzgemkbw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gtqnhozpp.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ghoclrsuq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gktwdxqez.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gbckulllj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/ghccamyyg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gzndnxkrk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gibvagkag.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gaihjjhvq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gvrjvtekg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gqtfgfcag.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gcwnwolio.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gwwzjfnsa.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gwvibxvkl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/ghpbgueiv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/ggnpssvzf.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gizclfgjo.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ggdqkbpxk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gqlzpakjm.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/garqcsxcm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gurwdigph.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/ggaxajxyk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/grnkapkxs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gjlvcbarr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/ghkcpegrn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbkfbhnng.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gsddsnfla.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/guemxabvc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gammqjcrl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gztrilfuf.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gwdhblqws.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqpzdlqly.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gsjetnfuj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gjorfvkwe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gaafqrczc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gobhgylmu.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gcywstxpx.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/guukseodf.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gortcljlt.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gioqwrrnq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/geodpvupj.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gfgvuqpye.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gafbyxzqd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gorvvimwg.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gjpubnncg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gukbtyphw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gpzgtdeex.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gybuhnqgh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gnughslxa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gcovjwkwx.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gffihyydj.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/giwpbimxy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/girzpaskq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gqxmmtvwg.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gpdtfxvkx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/grnemuqfs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gjziavvji.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gqbinihsw.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/ggvdzjviw.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gmaboruik.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gmmpsdyhn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gibocqnot.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gnscgyrix.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gwisyclxp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/ghydyedcv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/grqtibtbp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gcedrbcqy.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gdilkiawh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gswfrnygy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gvpklmpfb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/ggomnqbtw.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/galoswhmk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gikwrqgbt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gayfzgrat.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/grgewkvzm.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gfawsxfej.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/guffztnmk.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gewrwehsa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/grtfidtmq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gowwwygzl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gaatiphhf.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/geyiywjns.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gqxvwhpjj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/guglamfpo.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gsdlunlnj.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gpzesidfa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpmbmcffl.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxduthnei.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnerowxin.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gjlqxjkyp.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gjizsqqsx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gparfomqq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gmgceywpp.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gspljzngw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gocipbzxy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/ghijmyhjv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/geuzwvhfe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gfrxbrfcl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/goexjhnra.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gzbfruyka.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gggbnpgiz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gnhswcnyj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gdpfxsvcl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gibreowxn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gxtssopyv.sHtML


<!-- 参考信息 -->