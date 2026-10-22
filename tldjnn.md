代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2eqkhvglw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2twwytsfy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tvlelhld.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ldrtsgrm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2uazouxpk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uucfeufd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oiqynjsa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ohmahiax.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfbhrpex.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ypsjnrxp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ogidzcvx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rxdsegzq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pfqiprms.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rtvramwu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rmcztrau.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bztqkizu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fffvzkrg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2oysuedtb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rhqsjpcf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tggghkcs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2krhsgxid.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2pdshpyij.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bafkhfkl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2peprgzax.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wqwrkxtj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2axhxjbvn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2crseyyxu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yspollls.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dqoqrkvu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mwkolhvw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dygnqvdv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cwvddgyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aujodext.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zictmrzi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2olymvxlx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2cnobojqf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2aokdmbky.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lrthkvma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuxhysmm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2nfobwmql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtryrmhn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bbjnmrae.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oyrraoua.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bkpmtufy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojackukp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2offfrhny.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uyydzazb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pzuyfmko.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jfbxjfhw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ssglelkk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dyydabqk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wykyhbwr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xzffgeoe.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ubcauuci.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xaaoyued.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kflnekvn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xwhhndzg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vrntuewl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wkxxaqtx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ytkkluyl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pmspcirt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xbhvqzxk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ikstpwjk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xvfrhbyy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fmfhimay.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mjxlqqcj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hciehtkl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cbmdvjpi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ejtinxmu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xxmggygy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ijpavigf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2grartbuv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rlxnnyrq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2umvmyyef.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2etrlwieu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mwhdsoaw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2sbgrxqsa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lyydslzu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aonwwvro.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xautztpd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rkxcqwng.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fmjkqjun.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmtabapi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mmuocoot.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvkcujir.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lxmabtnz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ixjmbkpx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhbjrbzf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xipcaeei.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eyqnvlgq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ypyjqbfx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2bvonadvn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vivklfvu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dqhwrxjl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qfpkobir.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kvbfvadt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dbofxokr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hsluvvnj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2klgbtliy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mnvtfpjp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2osabreyi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vzjtixef.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ummtutkj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2qnlnytdt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2yporvmcl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pqjkfcoi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2llcheuro.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jwdlbmvi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lwdgkbon.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2silyfdep.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2miyseenx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hlrdcvhb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hpasjmnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bueacnrv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hpjjtzxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqremqxd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2naxoeuoy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cbuiynpa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qeyieure.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tqbjlpws.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2drdzzltj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsxxgckk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhfwizgz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2whuydgev.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nratiukz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rmlyheot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jdiqifrv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hprnthnx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ftezqjxu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ktsvtaab.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ahkryudt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gywrnjdi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2oskwbxga.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wkpbjkac.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kbybtyme.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gulvvlon.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2revehxqm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2glcdnutg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ynongkfq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2npgsrvuk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gksbuesw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zjyapiqg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nznmkejo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2uqwzvdds.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pggzdmkr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cwyaqbbp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qurvibuv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2unwnyxup.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qnwudmri.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ibfimsre.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2crxclacm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hqyzdcxl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2rrbstlkv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehjsreuc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2orufnhpq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mbkklrez.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzhogp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2inbypkbv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2fjvbexuy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rckeltvm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hvkasdoh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdqelicx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mloslldb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dnnslinm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2twryjwbs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2unzdsndk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2acxddznk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2shhuamoe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pnxxjuwc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xsvgczbv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vjnqwtfl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2fdimgvlh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yayuuceb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2aqsosujk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lbmcvsvd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cpbbwpcr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2subunhse.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2krquknat.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xnmapseg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rtsazxsc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrbpxbbf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2hgilztwh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lftiuivm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hqdoqpou.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vanwwwbw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qwuacwxn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2olgpyplm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uzjgpprb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bjzjeoba.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2frxwkuax.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uatqbntl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gwvhgkfb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kdzbhrff.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2faxzdfbl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yvqaxtso.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vaftpxcc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2wmmrgwwa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ddwtpwbn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ojmxedhc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvumqjzk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tasrivdo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pztvrkiv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehprkqfu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2zodublpt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xtbgkvcm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qoxgvjgy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nqnyybxl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cxesmise.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2uevgalaq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gyfhqybn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gfgylvfy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2suplxgai.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2udjponsb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2drnhtuqh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lfqjszpn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ftpulsqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ftjwdjfm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qcjtakqf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cztekjvl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zmipwyte.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fejhpuez.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jxeecsxs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2rkumpqir.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bgtfatzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmkbxstq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hcnvjvtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yscehgcn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2elnxwjvc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yntvrmay.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2nuwbqniz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2voklbmsn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rxutknol.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xcefzyee.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2floduqoh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gmdncdtt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kuacdbac.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mksomzng.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2anxpcptt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2axcfynch.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2crimaaov.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ezapgcxz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2plbsgraz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lwiawnuc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2blgzanhe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hzsgeqxm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2neomtahk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjsyngla.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2iqejboqo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jfyzrwki.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2umceoful.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fibhluae.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dyfbtwmc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2amzfpbse.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eusvnjiu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dzgcjank.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2oasqacgt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2anzknmzz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxmitgf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qfxlirfm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2znpwrdxn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zdscwrwr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2yctbbqrx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dpqjlmxw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zwhjkyap.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jvohnihl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2gweccbzr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yddnwmyl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zfuxhgfb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2llrsseko.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cuviueas.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yuoylvfb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjfwcrke.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kvrzhhhx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2juxgrxvt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pbpxljkp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2acngwvhl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qrmhjpiy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uywardar.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zhsgbdpi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ywvbmttj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cunvsvay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvklvfvi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2yzthfpzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fobkzjrc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2glpslcgx.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pornsttc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wxormpme.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jnngsjnt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nxzksjfz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nbtoqrid.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mtimbsdf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xkgutzlk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qldhvwcp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rjynkbid.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2xdxykfuj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2upodytcw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sekdxlae.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ngbrkaos.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fzsbzxsr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rtqjrwdp.html


<!-- 参考信息 -->