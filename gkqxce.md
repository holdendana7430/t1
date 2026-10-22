代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bdzavaeb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2uazqafac.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jxabkdzz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tbsuwgkq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dbikwccx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kbckqemb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hjoqlats.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nvhvxjrx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kxmwldvy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2glpokdxl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2crmdvvrl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2htbilmjh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2uhijlzep.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jztelyvb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2imnaykle.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ynyqwnlc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tsqngmvc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zmkuabmb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rkheoyyv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rlcawdgv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2silzuhma.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2tjfpcjqa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mjjmjknb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pasltjfz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lujegcpg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lyohxmde.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sjjthxyd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jpuzsicv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2deizvqdj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dxlmdhmf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vpohrwlp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jnqmnxoq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qbcwaodh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zpipljel.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rbjzwryy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zwswufyf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2njgbsgbt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2teedndkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thxnqpsd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dowtysiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bevmtxsh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cqrbsgfi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2narycmja.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hqssjfeq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvnjwyjh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqqxflpd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jsqxytsz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gbvdreqx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lhoovtdv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gqsfqwos.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hdlasnkg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aabvpjia.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wjuwtcbb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wrswdsqt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hnjeveoi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xxhyujwr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yrqwroav.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xtjhjctk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tbdcxzux.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jqybhfbp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xhnvladv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lkkwyftj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2titicqgj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wqjzidbg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2aafezwlh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zjzcxrwp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rgrntfta.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rvvowiqu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xwypjony.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fapmadow.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2eszjxfwo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ojalmlmz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2shsppdqr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vwxqnizb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2asgshbta.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ggwoimru.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2pexucfxd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2eqmjjdbi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydjunzmj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yilmassr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2obgxuxiu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcgnhnub.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2asgibquf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xrylygpw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2afbvprpv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cmigppzs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lcoozfgb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2frkjyhdp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ayxfszuy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xecrdruz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vjyjyjvj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dcalmtwj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mixoqxtc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vggaofsb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fpnksklt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2plsnmuei.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ftpldvyg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2krkblhti.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nyowuexi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ghisxiem.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qfwwtozg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2dzlwpitd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2clmughvp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iunklfhv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bshlmvfy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zhybrovr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fueaqzzf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tlnzcyfv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zgjmlbku.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nizhluch.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ubvgguwg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vzfwqtbs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qemjehng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmnzhmqo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2stovdiws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbdgbqsy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nejayvyr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxlwnou.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oxjhporf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2buumzmsf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cilpvaiy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uusezkob.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eedvgxpo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mmkswdeo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fpthuwbz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kywzjrtf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gktscsze.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tahfgnke.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pcnuebau.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kiuqtcyt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2fksuqhvf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mhtnxoex.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ghwbknhw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tijqcknn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xjwobteb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2suotsjpn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xwgfnkea.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gsgnunae.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lzvgimiw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ugcntcrc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wyhkrytr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2rjeeqqzb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rxigdzsz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lpjcybru.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gcaihfpy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cprjfcwg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mnxxazvr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bmpfuhvm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2epixwvlg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2otpczipb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uotemeam.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zkfmfgte.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2khikbthd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hzpzuehj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iitnlmmd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cidjzigr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2myrjouzz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mdpljhyb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2iwxocqjl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2idyfzrtr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2llrvrijn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2oyfmzong.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rmurfatd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gepsvtco.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gtscdrwp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mhpzpvms.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2eetdiybp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2piduhtbm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pclciocp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wgnupkip.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lctikerc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lopcsssv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2baxtmims.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ugwkzjmh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2igpzcocd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cxueabeo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ehwjnejv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ndqpjqui.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fxdbicmb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gqfsjymg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tgfvfgxh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hsxlbqpw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dqntxbhf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qwhzkxcr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2smgsoncs.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fifclatm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kuiqufcv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2faoexnsf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hgnixjae.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rvlpflpt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrygnfuk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uzbxnlii.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vxfpvuly.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cducecuk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ipfgkzvz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hsucugnn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fkownahe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yobpcrel.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bkgoxfqr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vfcnbwxs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tdrrnokp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uttujhje.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lowiecpj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ubuwozho.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2isxocjsq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qywexfzn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lmtalfmw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jbllsobl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2quvzgkab.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2crkjwncs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eikophiz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hcxpfauc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hephwnpu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jlegwrlv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uvovlluo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hkznbpmo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2flwwahef.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2sitgcvrp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ucsgvdqv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ntripmfx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aeiyuqaz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nymtswox.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2aqpffshw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zavcasjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqqwrjci.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qabffzvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ongbwmqf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xndqnbsv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2emzuvxrd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2kenbygpt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nzpckeop.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2psjemdwc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vktvxwtd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jsyvllpq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ynkulibr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qlgqfcmg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zwmejbnl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hwumtzoc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2unxbrere.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wtzhkeee.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ymvzvkmd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ghlkmzpu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gmfatmcl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gdwpchei.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2gozdtleu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dvczhcso.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2usaqlbce.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lurkdjzs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nebrzdgc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bocbxayr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bblkcfdu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kaaiathu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhykpka.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wvifhgrd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fknuilmg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lklfdprw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2btlrbkzz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bkvuvmcu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bpuypcmp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2laaonxnx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fvfcmwsc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2gtfiyklx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oupcjfvo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sbjinfoh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vfgbezym.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fqzitzui.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vwlxejsr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2glvbxdpf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2tzcujwed.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vjekbbsr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vczndrat.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zwkxxltf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gswxcfoz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dnqqfdso.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2akoconsh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xklhivwa.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bgowurbw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mfdizjmr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yejijzoy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2aiipxxxu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pkbdzdzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyehtfid.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2whxduzrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuwbrozz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2odptqxnu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2davobtfz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ariqqrna.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xfegvknm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2deagmkor.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qfohjrnd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2atytqhjk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2blcxfhdf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jsslpetr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cthrsqdc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vcecrhbh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sshcitxx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zxyekspq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pgiotgxu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrkbubr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2lsgxjyrd.html


<!-- 参考信息 -->