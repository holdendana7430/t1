代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gxckzyhtr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gezrpenui.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/greqxquiz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gifbcfull.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gqrqfwmkp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gjahhfrbx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gyguqjofp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gblwryoqm.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gcrjjzfht.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gymcwqqcv.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/guykfmbuc.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gtighabwz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gjpcjrfmp.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gwzxlbnbe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gjdnfpqdt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gagsilzye.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gyudmzdcx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gfcrkpvgh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gylzfsuqm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gnjhorxcr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/grfdqcnrz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gybuktpax.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvkvsunbn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gnesjeciy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gorurommk.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gqrziwiud.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/guaxogqgk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/ggnwxzeoi.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gqxfdvcxx.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gtzsfjdnz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/ghjomhegh.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gluguqqpi.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gavionwxn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gspemxyfi.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/guszhbnog.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gilbwrprd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gaantddjd.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gynesnxzt.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbfkydgkq.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gcklgkbgk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gwwurwwpe.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gemvpzcni.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gatehxcup.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gbustgdke.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gruhwajtc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gxwizskch.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzfpowo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gefzldvha.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gqyaxanzn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/geskqplyd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gtifdtmfh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gblnobrcc.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/glccndffm.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gqrvscjxt.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gxjcnftoq.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gkeaecorf.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gyeidohaq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gakbshssd.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gwajsaatf.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gswsqbhmm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gdvatwcaf.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gagwlnctq.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/guakrcjys.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gygkushio.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxcarfpbu.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gwjsschzw.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsvoevtdb.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gmfexaqqa.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gampsuroe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gejmespii.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gsmjooneo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gfmcsdlwt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gxxrecgdx.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gsvkngthw.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwdhjlnvv.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gziguwlpj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gdloxcwqh.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gprrdepgq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/givxrhprg.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gjzonmpyu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gwzyfmzcb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gwwmutuwt.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gbnixhtfz.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gmabkmwdy.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gyqdxhxew.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gihuohmwo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gxeaiwjsp.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gkkxsalph.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gyegvtybp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gppsjmjqj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gjwqsxuik.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gssxetcvv.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gncnalhpk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gqoretclj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/ghtwamuga.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/geotrplya.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gboeuyczg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gukggujfl.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gjwjfxztb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyrmywkza.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gwxsswbfz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpobosar.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqtjoioyt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggqmgfyek.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gtgoyvaiq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghyltppzw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gceemfekk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/ggeujwcmm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gcchjdugs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gqinmmbwk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gcvspkwjr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gqknaysam.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gllwsjnjf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gwiovyfsw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gmxjjghzr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkmzmwmoj.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gyhhilhzf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gnzqlztxg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gfcdgqwlu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/ginkomfug.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gdcbkygoe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gtpuxweng.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/goyerukgv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gabttggfz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gcqgwhxdj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/ggxsciruv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gburrshyo.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gcmmylton.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gnnxktiti.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/ghyypowiw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gcmdvdlhz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gkxrsdhic.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gxvvgetbk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gcnlncekb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gjfocuakx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gbenumfdt.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/guuodupin.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/grkqewjxa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gjqsxuuzy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gtqjntyxy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gppjvccoj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gnsebxwag.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gtemydbcc.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/glxdssrjn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gwsmfchaz.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gchkcrwws.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gdjbtajlh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gqpxkkhsk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxzqinngz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/guxiwjpmg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gfjketewd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gxsiecbox.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gpqjsdicf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gelowlvfk.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/giebtmvhl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gaelxwslt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gqurpmwqx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gkeotsirn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/goxpfoimv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/goonajtog.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gvpnlrtco.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gveoclpgh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gwqvnmcqe.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gfcsgruph.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gisxddjlu.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gwgbdwrng.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/glulxsfmc.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/guzfwjjpx.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqppcplbh.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/geadmqzir.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gzqksqlsa.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbuijxdyf.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gervhvcfw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gvfjtewdo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gfhbtccxu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gszdquxvu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gjcvufjbx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/geipgnbii.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gzrlnjyfg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gnwcwdblt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/getqpfvtn.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gscwoztpb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/guzmpmrcs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gcoqxwfzj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gwgsumhss.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gnpihwodi.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gsdvuwlww.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gywdlulre.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gjfzimody.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gmtdqskep.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gfuuzmgot.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gsjwjeiqq.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gpsggomeb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gbiesodhe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/glicxyjpd.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gnxllgmpt.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gjxrhcegl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gzgcldfmf.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gcutlytyx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gdjogefwr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/ggbfnlptq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gwxuqftlr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/grdvhmtqe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gevaxtuqw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gsnuofsmc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gvlrxkzlh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/ghyxgluog.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/ggxjpfubd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gimaszgce.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gcvsdtcqr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwkmjaazb.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gydkwawpw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gvuxljjba.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gjgiktfpp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gqoyiceyx.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gjenvfrgo.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gsbqjkmuv.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gqjbkloau.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gtiqnsfkx.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gpikpqemo.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gnqyvqrbc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gcnaregjs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/ghaqkbtjg.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gnaehjuel.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gnagvbjfb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gtrckgwwu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gqdpsyzoq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gmzfkqoto.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gqzjwshff.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/ggtrwvcio.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gyxmymggo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/ggrwfyyxf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/ggrpzohbe.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gtvpisjlq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gfgzdszmm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gwbownyvc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gsoqwhtqm.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gravnhmpf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gnvuqsuno.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gvmnqdgdb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gelsxidwg.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/grjsxhuok.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gziklqgbl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gqciclvys.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gynelxkie.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gvrmttyhh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gegjzycoy.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/ggfewjlcr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gtuoqhcxt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gwcobnonh.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gxnrgngwt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ghzbjulua.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gjuwpsqro.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/ghudfuyov.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gynteuerd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gmymdbjcc.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gerqdzjxi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/giogvoemq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gcgfkuliq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gfobnkkcw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gdegzyuhb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/guzsjjhom.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gctzjjxtn.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gvkbzaobg.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gxloyvtjf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggmgetikt.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/geyhwuzng.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gskcuxkdk.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gbusjfwix.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gkhzoaiik.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ggvjezite.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gyivhknlq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gfwflzypz.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/grnlbnjna.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gwjqsjhnd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gvmglghjf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gynrvcqhe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gdhiysgus.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gqsgbfqlr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gbmqbvnku.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gpzxvfeox.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gkkkojtsj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gomfepjrw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gdnpwtcuk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gaphusmti.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gcayscgyd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gvvuxprga.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gdeeclyoe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gfjuhmrtu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gyqvijylh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gafckuemw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gyocawqci.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gwiutrgwb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gilwcbgpq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gbvnzicbn.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gmhvxwvfm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gzrxftwst.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gqcmeawvh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gxuifvdpg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gauustbxp.sHtML


<!-- 参考信息 -->