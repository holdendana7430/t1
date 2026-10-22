代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2aygxhaye.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pdphqyqo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tcxqbbbk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jhcdtgqg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2beqtahcx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2flddewbg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nubqirid.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qpbywmim.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rdxyfidy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ekhfjsik.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dsuhpoul.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eozfmxdc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ocyfahro.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vmjzwchp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ephdvckr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hvnufqvq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fjdjsphu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ykrhtbwy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xqvhfiak.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lqzvcxfd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bmivxghf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ftewjyff.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qwebkzjd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wkhphuml.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dbsacsgf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2yiucljyw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bmfbncfa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wimtzwrn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bvvughvo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ecxumosh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xmtpkftx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vmlkimim.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zxiqqddd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nqzztjly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hofwjhqc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2usqmitux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aaisuiwn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ebecxvkd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2zmpgcixw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rtrvmnuu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gkefzisd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2quvptkvd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ciffqwfe.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2peklgfkf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2swkyskvj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oqtiqlvt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nictkkmq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2edpylrts.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2amzpxpmr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hlyssbxp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dffrdscr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uvlcsruh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tfzrlcie.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rxextlcp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yxzdxwyo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yilvznxk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2atgwlkhj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dpixuoxf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zczeblgb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gawtjxlm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tlsxamhu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ckvybkps.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dhssltma.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ucsihbde.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pklzcqov.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fnfscknu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hhyjdibg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tkyacinr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gebkfefi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tdxozbaj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2btbsiajs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2shmklzak.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zvnzueda.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jjtwuesr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uyfwfqaf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mtjwjhle.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2muebrqpf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2conindiw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2undjjpjb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mgdqzzuc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xnyefxsw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ughfwyrr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2sktqkeme.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vcfrikdc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mrwprgrj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2elrrtjro.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nxqssfjo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2detekfky.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pkmxefop.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2iormlbqk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vzcyhflm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uwbkqdzg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2odllqgit.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qmgimisk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nxzpvyae.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2juzihtnm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bxcmmeru.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2iwzopkox.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ngjtkaap.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nfiomcpj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zdfapejf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wtgwvdsu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lqmhvxce.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qaxlckux.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nhrodvll.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xpgwcoho.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gtvvgivr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2aisyreqs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wpthmouq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krkbatpl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2devhbhsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkbqcidc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vvelkdpf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bqgiawrj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bldvpgch.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iivwmkln.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mptsgndp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kybjqnab.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qoxpwedy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2iufjawis.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfoduuh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nqqrccfh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2csyzkvxm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uqnstbgg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mkloerfm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2aovwljsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uxcxrksq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tehaqlln.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xuwqyspl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mutbteyz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cmnepukl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2afeimghm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2napulbga.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pkrtnysa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nelbugfw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fanfxfyq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2oeqboopp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cuanmkrk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wqpadzle.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2iwmdkfek.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2addjsizm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vaahlrzh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cnbajvdq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dnmgcwql.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jokilhar.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mapoenyb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfppctcj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nhqflgkx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2odepsxzg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ijnlkrst.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ocxarmaw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpmgmfim.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hesznvuf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ojyozqko.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2olbwdjsu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pwdaugtu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsdxwcja.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ilkjhajv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tkmljdxt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mnyzkynb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ptnskabs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lpgzsdhp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kbhetrpg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2krqwwoxq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dzsgxwan.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hzzirdlb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2npdsfmpg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mtynyewq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2umfgmxti.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xlwpvhmh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uwzeboqq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2eqozwhuc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vfmszbwr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zuncyffn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kbjthsoj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jyqbcayd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkbpkgix.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2yckwafcw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mcrhrigp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tmvlplqr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iykttogd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lrlvhbet.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jdendoso.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oobjmqnm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uofaiaal.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xrmhgupk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ddrdiqyz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jiyewwcz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ikzrycoq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zideiknm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2tkvvpaxg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ynftwvjk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lkdoerkm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2idllapax.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2eompkgaa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcyrlurg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dceevzca.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ywemrsvf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hnjurnwu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nzchakcm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2niuekfkq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rgjiwmzd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hwjmstjy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2tdxxxltw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nyrhfstw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bwubstqj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cmorocvj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xdkbdlpw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lebhdntr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vykqdwbd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ifdhtxqn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qoedolqt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fkdmbkvh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pxyqlawi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dwavovhx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qzavkbmx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hjkhailk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dretvxdb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2uvggeclr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2htpuerey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybaajfgy.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gtibycji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zniqicpv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ywslhobw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wwldxkck.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dhdbjnyc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nrfmlthw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tjoyoozd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2iswnhsqe.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tjwiiatb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nmpdxivf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2quyadovh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qlnabphb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2nhlbbtro.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2awuwkejj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ehtpbgdm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lumgtvzw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2odqhmile.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2jqzsmlph.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vuwykods.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dsnfueuu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ptrznouo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jkopmlvb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hcdsxdha.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2fjdjzxju.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jtxlwura.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqcxmcea.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pgtcaapw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gtaqqevl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2csivolio.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zqimavwh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zlqdfllb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bdltzvwa.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2llpvmuhl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgwublor.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2goqggwwu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2tfgmligm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fpszfcef.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qmfpkorl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jzeouypv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ltugpjmx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2anplklgl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aexmtsfo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fqxkknhf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2kjrxsewl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2uxtqivkw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lhyjuudw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tptchksm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2shqzddtw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2itegcdwl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rojkdnex.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cbsrnctr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2giusshhe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lurwsibu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ptksqert.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gmizkzon.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hshhpxnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtmbqjqf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mvmkcqiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2westftoy.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ooktgupa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nngiyvzs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2idibgwdd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2scmhrljk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2npdmmuxn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qazduqbr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oipqrqhj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2arghfcpl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2olzvozbs.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gkprgxsy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2abjrvuut.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmysuhje.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ebtxeklq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2awetspyc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dbzbxpiq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gpswhtzs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yibqqbpy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xrpuhcck.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rjfnipyb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qtlrdeta.html


<!-- 参考信息 -->