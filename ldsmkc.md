代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpjnjqhw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pmrsxsxc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fykhvwhk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qmclizow.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozhlvlib.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3fkvdxjkp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fbtvjdiv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pjryuopr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ralkknvj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kaytdmce.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zkfolldb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zvfbkbqx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3clpysfhl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ntzkuxlg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3vfpmkesq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3phnonaeg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3exkgnxxq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dwsytxyd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vivinfwz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kivukmsa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3teglypog.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ltawjfka.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pfefrcey.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lcmjzaqi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3itxgfncj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3cnmmhnur.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3clzxzeqf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qmprmukz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yjhfbqoz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uslbdrcn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3sfreghkj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vkgrmfmy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3usxlgxcb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zgmcheoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3norywnqk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lohsxokn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzmifneh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3soznbiqb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xwndvxic.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qjwqmeza.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oprfvkuz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkwjafnx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ocskbvir.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3oitzfosz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tsuoqklt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nbbmsmyq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fqukhntc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qrpgkxmf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kkwbtecx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dhvnpgpr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xutjkfpz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wlkhxxor.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pxaywvan.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jjxpfwur.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qgsbbvbx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3dfihblus.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3egnjavjj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bwyrvqpe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dtqfpitn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zhzzrrci.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jfnembtf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3twcssbke.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ploatctc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3oieeheib.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bnfuylpi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xfrgclxt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cpuvjccc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xcnodgcf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tvxqyxca.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ctxdecmk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ksmroxmm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kjskjcmy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jjnpvqky.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3miumrirv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uxfhgaph.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qvpfyhco.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwkpvwie.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lhftzwth.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkkoegce.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3leekwwjo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3wsmwpzwd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pucejjra.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hucotflv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jnqbhqxm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3okevfwhi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3takoyspl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fxvzxofe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3shqxnpgu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bqdoywkc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qveyulet.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pjorhxlw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dbmvevvn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fedzoxto.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qfpolped.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3spxgtzzj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bidgpdlo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tmlmjqyq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3yngcogsi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nlxsglpj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mtvtkmkh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3myalkjlu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3amgnsmyc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3htpvmujj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xaegctwn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qcpeamrc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lizpdqpl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jjfqmlho.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tefsnnhg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xjpdytzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qoxbpdum.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yqmyafik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wevysren.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tmkkmhqz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xzxcycjf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ebvaimgq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vzpajkna.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mhytptul.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rsnctrjh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrngqjyk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3spldzrep.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejxwvdyo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qygzcdbi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hazvujol.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kzqubvlg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3myvmwcaz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ammydyvl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qzmivcdh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwcemqr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3popuclby.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wywtumry.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3akzefkad.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qxxatoze.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3zbeupxoo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ilrvjerp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qhgamdml.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jddovkfh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jvnwiehz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zalyvmue.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cscbfhva.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ktfiifnu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjegetcq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3euicmhsu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rcopdkst.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jqqbzccw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3coqwxknq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bawyflyl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sqnbssdt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ewholunc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lmfskddb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uwowimbp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhxymthq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbkbojyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3luxcmdla.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tgweutgc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nwhozjzp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rjjyyzno.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zsieujrr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ytnzhrdh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oryxiqcw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3otrwihwe.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jfncinub.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tyslzaah.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gorvxydg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ktlbkedi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wmgcbsce.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qodvkzqm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hlbbmupj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3cwvoklhl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gjfntcsa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3pzdpznxf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ihtppqpx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dheeecwl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3eyxluzno.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3qavcuvre.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gbpwcbsp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bnxzhlzr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cxxoaoqr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3calevein.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jiviuztg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wdohvrzz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eialkitl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vhbbezzc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zsjrlaky.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jepwnngi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fpaighhx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tpydelxw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ufhuwkvf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxailtyz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mogvuhho.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3blqlporo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xqyluvhc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mnsoocsg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ynielnkp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qxrwcmye.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mefxbvgf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3yfvmowng.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qaeugxpz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xzqxnzlc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3uhqnsiyc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3neyhhiym.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ssnpocjm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bwvhhtef.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ypmpcvwl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3amkcbgjh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3eungxykp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3reiocstv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zccqjgfh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dslqogum.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3conykzik.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ebetqzkw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3exdurcbb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ecgtowkd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xohtrmug.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yostokkp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wsrwikuv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xgirzlmc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jamgpvuk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qhkovfps.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bpugwxxp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nuijooas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdsbtqko.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3psdtdwwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssxxwoqq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wxighymh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ttnmavok.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mjzheaer.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cshmwxth.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tgzemyds.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dijkveac.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3lnvnjdzs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zqheeptp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ayyjwisi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qcuunilm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vdktkqwx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qdhioatu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3glxfbvxq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yylbjsfi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rbwrxmwz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vcuyeisp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3psznynqq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3juenveox.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gdxuqfqp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mindwuhg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3eadwrzxc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3tqcqmxqg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ylitzkyr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnvvyeyo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zhzvmbld.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mhvrxtcj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhmbqduo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sxznawit.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3cetmzvbt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qkhkjnef.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljitshnd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnrtykcj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jdsdqwoi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wouqlsdu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3igciqjep.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3grhtghbv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3crehrges.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3saourikt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ceqhzuwp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rthbgiba.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bxlkksnw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3aalzniok.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vydrnifu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzpftre.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3dptrkagd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cpjrvtqi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3enwiqhgk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hbrjlsvx.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nqkcxdfo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qxbltoao.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ntqnfmqj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rdiuoqob.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rnrkwune.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ejcbmrnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfnrgkyr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3newebjsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgyqlhdg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nipgfyuv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yzuwloof.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rhmysimp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3glrxthyx.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kwfhrhlj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3coenbxwy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ngcfiorq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qcxyhhdw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3tucswjkk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rixhvvoj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nutqkqay.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wdezhulp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3sufoombc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yeynleux.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rkqscbrn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3letbrlwq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlpjuigf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nctwxtdi.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zqtutmfx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3efoiwvuh.html


<!-- 参考信息 -->