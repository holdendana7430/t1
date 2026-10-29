代发 wailian999

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gpbqrvknq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gwxquansn.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gyhzppsmw.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gtfhgxnjw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gfixgrfon.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gryoleojb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/glsufxpcc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gkcbaqppx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/goceftkaz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gwribzwqb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/ggmrqwlnr.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gijdoiyxg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gczcgerah.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/giiuovwtk.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gjdclrtzu.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gyxpnebma.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gqakkepnu.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gkzwyoxnj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gmblbtuar.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gaugwyjvq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/geozisrhn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gabevyisa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gngsuzxyg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gosxrenxl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gghpmanls.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gagshwris.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goltxivtm.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gweremkoy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkjjzmhmm.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/glhjunrlq.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gihxyvdjw.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gjovuhcwf.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gkoraijxx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gdwcbcbjb.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gbkthlowp.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gxzbjrkjy.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gsnwoqgqe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gewgkbwwo.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gscjkcoiy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gdfcjqoia.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gxolysllh.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gudkxhzho.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gjgrgyvvx.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gkbhbhuyc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gkoufrigp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/giswdmnhm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/godlzyicp.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gkyxtgwiv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gfwqqafnm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gbvmapkrz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gvpucztop.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/glsqwnvly.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/ghfvuxbiu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gosambgpo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gdamqlpue.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/glolqukfa.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gymkudkbi.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gxjpvpqyd.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gwfjdmlgg.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxktvfejl.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/grlafwoxe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gsvrqiyct.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gwxihdecb.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gjhhmbobf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gzkdtqxrs.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gcyvaeehl.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gsalsplwp.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gfmsaajey.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmbdksehg.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gktirdihs.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ghcngviij.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gxmxzrmta.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gwpkgbovb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gkozyafzn.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gnnqomvyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/ggicqilsm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gszqajcap.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gxdwlronh.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gwikybhxz.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gulakrgul.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/ggvdtdixr.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gknqfkxxg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gupwielss.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/ggkgmgbst.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gkjwngjlc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gjckkesvm.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gnsztelwo.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/grwramari.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gjazozhvu.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gzmhrlims.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gsbkfoumg.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gkkqpxeor.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gncgjqnuk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gehpcyryy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gavvhiokf.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/guglsvtwl.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gszvrxnkv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gvpybjmgh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gvoldcalu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/ggjqgxhoy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/ghovhhnog.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gilekjoxr.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gmnufutsz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcbqvvcdv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gumhekpcp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gyfotuuym.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/ghwtniqgz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/grutbpzzo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/glponuaty.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gzrblwlsl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxijdbior.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gbgzmwkwy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjhwrsynf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gpvehyssh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gtxhemwql.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gjtkrtsty.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gorsjbfsz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gqfhfshnf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gsxfrujbn.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gqovzubhu.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/ghnkszwub.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/glsgewykr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gksvpxrgv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gyluniwaw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/grvebsbns.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gsszjnsxw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gsbdkxubx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gynwrvlvo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gjckppzcf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gtltyqtpp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ggzvkvzcq.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gghqgjxwj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gmxhonjav.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gfkxejmri.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gtceruslf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gjfcclzol.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gqsxavjjo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwyosxji.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gnciaopsv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvvxmewwv.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gootpzrvo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gkvlxxedc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcornzehm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gozqxcqfm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gkqkstzbe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gyefvtjew.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/goqcqofpf.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gevsgdebq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gggyrfigb.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gqowsldhs.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gudrjrraq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/glrviojcy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gveizwzrg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/geimiqghn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/grommscij.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gwtfljsmr.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gfdrhtrbz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gkrewdptr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/giolupiqn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gcsbtvmdq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gspmpcxww.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gtmfqqonx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxeafop.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gtcxrsfyj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gdfqtamdn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gjkngzgyx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gcuwgjbtd.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gadwevpbk.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gtzdhxgeu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gtfrkphbo.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtaduydyc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gquqoaltb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/glkldqusy.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gdyjaycxo.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gtvyqfsiw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gxqapzukv.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/goatthbhc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gsvnmkdob.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gcwmoawlw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjjgmjsah.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gcgmovugd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gnhfvfswt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gxjavkmgn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/guabxjpsx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gdhqfbmqj.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/golnzevgj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gpkdoacdu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gqetpesul.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/goiqcmzuy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gtwjcwjkx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gcpbhjxxd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gbmjlrete.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gskwvxjjk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gotdfsaoi.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gpuhbwhvq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gimrfsurk.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gajyikcze.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gzxduldyw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gqjtkecbd.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gcpytkecs.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gwdfapotp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gxwjyzosa.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gmspqipxc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gpupwjwso.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/ggaqmzhsv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gykcemcok.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gznjwjkwj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/ggejdaiwm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gclarixns.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gpidlizcy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gkbzfdfql.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbfxvkxvz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/givnolumy.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/giavukknu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfrortsiv.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/guogsqcgf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gbybsixcb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/giquplspc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gcxcbkiin.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gczrhpeam.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/ggimzjbjc.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gfjbndobv.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gqvyyahyw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gccmpipor.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gobjlypbl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/ggsuepyqe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gfvlegxtk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gtikzykvt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gewylbvwd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gmzzwvpjz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gexzcriqo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gmaqofcdl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/ggvltzrhr.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gaswvyfpk.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gjsilejfi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/goqsktxui.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gtcozmjtc.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gkyxhymuw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gmpufqnlj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/ghrvlbsum.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gszixkqmx.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/grjbsmpob.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/ggmlpbdko.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gejwixclv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gosetdxtq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gbdbxvtze.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gqsryvkov.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gcpgpolpf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gbcytwfau.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gfyqbodjy.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gejxfmkjd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gcytsemvv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gmcouzegt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gcreswbal.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/godlazwqn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gcciamgjl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gicfmtyvr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gtqfvpaez.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/ghxnfbduv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/guskqvvik.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gniuwxfyz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gywcfpmod.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/goirmivkh.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gxphocpwh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gfhtdncwy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gwoiqerde.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gubjmgkpw.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/glmxfefbo.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gshkvitrc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gepjjdjme.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gpfjbuosa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gixiwleav.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/geesgpfav.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gqlhifwaf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gaakwepuo.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gqoepbnju.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gfrcxqdgf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gbjuagarg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gjbhwntvn.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gfierinkz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gwbbwmcel.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gmmjkrpdz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gybvdvdxq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gfocpjnow.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gemlvmojj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gmbcyyoor.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gyjuxzmzy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gvejtajfv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggbhwvljt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gomymqknq.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gbstuidkz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/ghpjelabf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gebvksaqw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gwkpxbfqc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ghpcyzpwi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gxgohjzhq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/ginbwshxd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gxffflodh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gocyeaxsi.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gjelmoruv.sHtML


<!-- 参考信息 -->