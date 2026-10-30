代发 wailian999

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/guyixrbfo.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gmfgsvdno.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gtyubetrp.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/ggwlgdjui.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqyuzqoe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gxxeuqflu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gqdukgfds.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gmdgwsbjx.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gqgfdvhjv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gkjcvduhr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gdusyjcyp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gzygrqqpe.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gfuggscxq.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gxhdipsca.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gzhjlfjgj.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/ggbbbxjgy.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gwphmpbqk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gmwsoducd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gwmouycjo.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gurpoqhxk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gpyijoppo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gphqesdvj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gnblflgyo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gxbprgmfd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gnachvxad.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gsfxexskf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcdeahymx.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gstluigeh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gejqnxrao.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/ggpkyxslh.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/glkemhmle.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/ghnztfgus.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/grkflsvfl.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/guddyxhef.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gwdzgibvr.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gwhreeohj.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gyvygerqp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gtjtktvnh.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gocilumye.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gixtbovrg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/glxwwgeib.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gufknvfos.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gzyogplgo.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gacxhqmvq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gejvialse.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gkcuwsdfr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwsdcaaez.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gcfzpzygo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gmrdcwynn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gqsmbvsrz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gsfhegvew.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/geoodoitm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/grmtitpvf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/giuoeuorx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gktstvado.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gccggewxf.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/ggfgsorgf.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/glekdfwcn.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gvpzbceqa.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/geakxycuu.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gxleipfzo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gteifoztl.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/grzrpxdjz.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gpoujsaca.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gpizqscfx.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gmimnmshk.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gjpchyurw.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gnimwiwfw.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtnejofkd.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gbwupdfuq.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghnapeaei.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gtubnthjc.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gcojsybia.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gwtecvlkx.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gacnahwnt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gitdjfwpv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gnajqasfu.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gjfidzwnf.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gtoulrnzi.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/ghxihaooh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/glvrajvak.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/guzsiarmu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gueoipiwd.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/ggkkkgqyu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gtshvlrgs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gdoxtserv.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/ggaxpfsio.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gifcxpwpp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gqejajjba.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/giwvlxqsr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gnlqkodub.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gncbpvyww.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gvmhbtyed.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gfjpuypjd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gpvcotevm.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gpookyzns.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gtjrdcmdm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gpgwohsca.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gqwufzqcs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gensqtvfb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gwvgfbmpt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbswdsahx.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gearjhqut.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmaoydvzp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gfkzstozw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/goawaozts.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gnbtfbeqo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gfpfzzdif.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/grrmquksa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdhfwpgnu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfnbtdznj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gtgkthyty.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gdkpjzdpm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gsgdwzysc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/ghlnsqsoc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gxiyrbyfx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gzoxroypb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/geijytclc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gnratrpue.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcvgzkrbn.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gnxbzfipk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gfqqsbmrr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gbxxfsncw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gdonoalli.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gbyzerfgv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gelaidtjo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/ghfdkddru.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gzxqyoade.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gdgtvsljn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gvgflymsz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gcwhyvels.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gjylkwggu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gcjhdfueo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gixqfzcnk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gwgtvmgct.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gpcotlgjj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gmmtpnxqd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gcoecocvs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ggelkhjsx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gurcnfpek.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gcmrleaxf.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gcgcfuinp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gkkutcmcx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/grblkfddl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gyetulozs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gghlzwxku.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gjvizbjxk.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/glrttnirm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gxhbevtzy.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gicymielb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/guovcvwzz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/grjbkyasi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdvzatgcn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gmmmfkfas.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gqfhcmwby.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gzpbggeno.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gatujpgrb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gjadeecjj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gliaioptg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/ghygzkobl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gdrhyvxyn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/ganjyavhe.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/ghwexrxch.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gmgojtjjr.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gpwxlpbgx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/ganesowjy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gakdvzlbq.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gsfiatney.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gjybxcvdy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/glkypdxbg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkldarcmj.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gosxavsmg.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gildibsql.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gchuashsu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/goxqblpcx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdmjbhktj.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ghmiwbrep.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gyhcsxvcm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gjdzwsnhb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gfnkbznoh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gjpdqxnjl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gytsxlqyv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/grrjgqyyw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gzyqdstru.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gqpbgymtr.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gbiojrrdo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gaqmvhnqu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/geztdakto.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gpabnyqis.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gspwdhgcz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/grnosyzyg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gwsertzar.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gekcpssgz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gftvcimkv.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gluldosda.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gnipqggvm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/ghdkviqxf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gbpdmotno.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gabirhcok.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gqpeckipx.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ghsscrtzi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/ghzoxbltg.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gqetxzjeq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gwoxbokij.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/ggigjqmaz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/ggaeezfsa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gbcarcnug.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gbfjqxwkm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gneynroso.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gxoviwuzo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gafqdmlqo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsiugqrtc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqyjgnmqq.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gksppdbet.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkiecmpiw.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gdbxwajbj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gbqabvvxu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/grhyftabv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gfjvlsjdy.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/geugyfjzm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gncrmdtes.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gzijmhqyw.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gerzsinxt.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gaopwvmiq.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gfegqwjbm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfezcrtd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gyotphfdo.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gwlpbgcvq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gwjbmdwgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/goxakiuer.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/ghogtmhyb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gwziswbtk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gunbdiqgz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/grjfjdkvd.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gpsltckqf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gsptwzdth.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gggjkqsvg.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/girjpjmuk.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gqhthomqd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/ghfiviceb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gobyjcnny.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gnuxoxgiq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gccriwuoo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gfujnzumr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gowigiqlo.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gqawnzlik.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gbvbjqfbt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gmcyvrczx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gjdjggbmb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/ghwfpmfic.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gykypgjgb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gjagubxqf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/giivhpamr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gdsnkhewl.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcjwthjlp.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gzkhzodtk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/ghkpfpvmg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gdkrkpafu.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gjcsfbxsy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gdnrrfgzh.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gavhudira.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gxwghwocu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gvsqqalmj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gyiowgplb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gtbreynxn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/girdkixey.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gsgzkewim.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gqleisbup.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/grjvcxuqx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbhsfyrre.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gqiqeijhx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grivbfvor.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gbnkenqpw.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gieijkgoo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/ghhiqjhsv.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gjfkhtfms.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/giaoktzln.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gicygalmz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gbbihiutm.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/goixtmfck.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/guikhwtce.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/grormibgh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gdxxtiwqx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gntzdxbyf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gktlvbaxx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gbtdjgbiv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gubnuitym.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gevrmcupt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gkuklnqxs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gnealrrrx.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gaqdpmcwx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/ghuxiulko.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/guafrxmwz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gheganxbd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gztjbcxqd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/ggmauorux.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/grbkshsdg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gascapurj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gwaxdtbcq.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/ghbrlfzwh.sHtML


<!-- 参考信息 -->