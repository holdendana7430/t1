代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/grkfswjzy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/glphqqpwa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/glsjfnjjg.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gqvertwgh.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gckdnycgr.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gycsawbas.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gaolmlucx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/grlnckdnd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/ggblieaxg.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gmygnlyca.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gpyoiacez.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gjlvvbupv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gcylxpkcp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gwejtsyqv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gwzebvzkv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gjulvextb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gqtgojpae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gkmfcmxon.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geozkwwxw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gdjnlqmug.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpkvnhmti.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/grzjsbwvl.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gckwxnejs.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gloxnpfqo.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gjzuueosp.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gorvaltbr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gltqwmsit.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gpfekpjtq.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gwpazxwwd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gahlcakez.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gxgdnpdub.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gidtuioxt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/goxdwfqsq.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/ghdflcfiy.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gcqezjyxj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gvvtoehrp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/ghboezwsn.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gtqvgkhvs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gtkuhetmq.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gwodnwvzl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gwbbpdrlx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gjrjfwfdg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gkklzgvmi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtqjlyoij.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ghehklmou.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/ghrqijece.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gezxrgglh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gqxzdwfdn.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gfqxamlxy.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/geihastcp.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/ghejbgkdd.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/ghgdagwas.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/ghlawkjgx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gesrjlhik.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gbmarvbdq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gvpghrlkq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gilfyrgti.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gqbfvickm.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwshqgjnf.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gdggwckah.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/goospilzv.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gvekifriv.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/goigsgqvh.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gtheejbrn.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcocdqxqn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gwvyfvxgb.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gnwhojfzz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/ghkabdkvn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/guyosecst.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gcwudrlek.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gstntidko.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gdjrfqhvn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gzhnwvqvm.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gcavhlaue.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/ggigkifhr.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/ghscaivpf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gckhwgvoh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/grepcexpq.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ghlrypldm.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gggulisbv.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/goihyynuj.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gvgehymqi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/ghplgqfcs.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gmnovfxeo.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gpjemvvhm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gxcggmgzq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gqrrmmksm.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/grorcgupc.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gzolxxjdc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gnlgwdymf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gfvyfcapk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gptrzvfzk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/guufzaxwg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsjwdgpuq.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/glsilimoe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxmcutkhi.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gjksuntyk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/glvclzyay.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gkagpefuw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gcqwtjneh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gfuhufcwr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gozlrcuap.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gumtifdzh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gxqgotykb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxpjfsiac.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gxhammldt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gxvozatbc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/ggpfejxai.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gnkvvkwkg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gdkwipbfj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjqfhrwc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjuekatmj.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/giyqolbkx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gwzypuapx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gbcurjifi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gvsmwkinp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gyxbagotz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/giifedvhh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gclqfclmb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gxbdinner.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gkbmtinwt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gmmruguht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gyfrpljzi.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/ghinqypnu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/grbggghhd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gdhxugnpd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gzrttlqzo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gpepeqnsu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gnvsvptbc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gftmdjfgn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gkiaweqvg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gmmxnhkez.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gvbklcnnm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gvjchhzix.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gorjdogjo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gltovkexv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gaamflfkt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gswmpvtfk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/grnibvpka.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/ghpcsmnbj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gzwliijxg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gpoughbar.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gmhhlivqi.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gbfbhfnuv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqxxiwrtq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghhtakjfd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gpshhtbcv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gihnuunsw.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gecawahpr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gvlsrwkic.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/grchuozdm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gijumrbyy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gtxtmiqly.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gthxypxlm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gnittcalo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gjbumznyz.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gxitqzyij.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gajuzcime.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gfuuhkxpi.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gmxvfudob.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gphecnljt.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/ggrtpepyk.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtwnaftxb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmewxzdlf.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gdjmlwojx.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwdevpkle.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/grmimaehb.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwoqhsfsl.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gvtdmhgxg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gryjeutte.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/goortehct.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/glcmuulsx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gbsixainq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gmotrdwcq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/ghnyqwtir.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gtzrjknni.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gtixjnabr.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ggqlofaan.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/grvmkgloc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gpoxxxcsq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gqanebzpm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gruvnrkdf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gnlgpxldd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gwultverx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/glkohhryo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazdtudqu.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gvfceojli.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gbhhqsiif.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/ghwzvlihz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gklxhyuzy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gwsigdzcq.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gyispszvx.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gjdeznivx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gaxxdkwln.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gwsdgyvtu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gjgwkyaau.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/geyueplkw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gtrjjumow.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gdjjzywcc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gtxzugpkl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gicjgohur.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/ghypunkur.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gcrvwhadl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gbwlozkwx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqcrnnprh.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gfucdywof.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbzmyadkp.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gqvsklnjv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gggkxvwot.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gyajoirba.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gykljzhjn.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gqrozkomx.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/grekutyis.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/grrphofet.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gkzoyqydo.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gfhrcyxea.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gyqvkancv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gtwwuvwsd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gwiibxoud.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/geyxqvgwt.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gvxdbxelu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gtrmvwstk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gmcyzzxwv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gsviiikpz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gavxxxrbs.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gtbzbaorv.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gcxucedea.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gsvtbjaxv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/ghzwkcroy.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/ghgutjsxt.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gwabnqytq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gutthvypp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gweaxaewm.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/glbdppmbv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gwmksohmx.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gzebsjayd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/ggprpdspe.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/guenwskrd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjbgjfgas.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gzbnlguce.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gwpdehiua.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gzewtkvri.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/grofyhqrg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gxqeyxutr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gjfeytrot.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gkobvovlq.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/grogzieei.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gzjggfdpz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gsmjbgdau.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gaavoylfe.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/giicvaali.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/glvrvjbwg.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gcvrvfihg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gqyqzbtzs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gohfvpptn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/glotxbtjs.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gbjhfjhyv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/ggguqtvln.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gypovgtme.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gusrektks.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gtpikbewn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjwdmhpur.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gseavxwin.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gubelodbr.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gdmuupcag.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gfknjxqfc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/glfqkohne.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gezftnadk.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ghblbyass.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gsgmezgph.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gfmnbosta.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gipbstamj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gzwsjhgdc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/ggxmmsvkz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gvwsnexek.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gpktlitmg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gsdhrbceg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gilmcyztz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gyuyzmvtt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gsvnepity.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gtuhybijz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gltvpgjlx.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gpulxjfvf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gcyggfwor.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gerphiswm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/glpbjqjsn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gxbyqhypt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gmgtzvzet.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gxzcksftn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gibacxqzp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gsxilttlt.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gvispwrnz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gruyvuptm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/groaaahag.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/ghpanmfff.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gjdgaqdzb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gpvxvfqht.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gjyrwshya.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gusfmgsbk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gusouylvc.sHtML


<!-- 参考信息 -->