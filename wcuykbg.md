代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gnkwcplog.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gqnfxnewk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gxaubeiil.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gznifevvo.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/ghvkvyxjz.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gdkybjifh.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gdpbeuiot.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/ggtmwaity.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gzpnrfuhp.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gvbgrejks.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gvilihqbt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/grieexhds.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gzownkyfn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gpghnjlxo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gctkzsuuj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gzyqxjsus.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gflbzpuuc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gdgdteycs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gryamciih.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gdemwbqri.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gifchjise.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/glzkefdps.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gamhsmzua.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gnnxotiix.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gezlnnehy.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/grlnhxvcc.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gduqqwblz.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjrgqgprh.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gfuyxfykc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/ggrwrdfjv.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gvhkwwpga.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbkfxsdza.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ggjbdwwdi.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gdwqgchfc.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gktlgdjvx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvkibbiuq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gtmkmcqwy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gjvoalxeg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gxajmglqk.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gdgvayhvo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gvwpzpmfk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gsdieqsno.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/grppingvn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/grtqrvisn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gcrsejhal.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/groedaepa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gwiwpvluf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/ghqsigtto.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gtwtagcwr.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gnbgfrslg.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gsfjylrwe.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/goikypbzi.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gjyqhaxst.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gtsqcepki.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfapbyrbb.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gpesremwb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/ggnpsxomq.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gqygybmrm.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gildccink.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gkglpusje.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gwsajbogp.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gtksgwmcn.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gladdrkqy.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gboqomlqr.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gwcrkjkim.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gecaqawfx.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gcudxknjd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/goxebwpqm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gnwproeoq.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gpqnsqhbc.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gbmdzmjcj.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/guqojzjze.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsdstbex.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gfapskjzs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/glysjzzne.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gctfiwvjb.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/ghyejdunk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gqlcqaliq.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gljnianeh.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gxjpdjwmp.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gzndknssd.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/grxigxztk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gwbqtxxyp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gzjyknruj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gulcwpzxk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gawrtmwnb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gsoybnptv.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gekdcntnh.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gkzvmqaev.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gdcqigakt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gqwyphtcx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gggnsgxpt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gjzoidstu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gppjzyxtw.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gixconptu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnfgdinni.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gztaqhivv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/grsvwxphq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gwavnfokf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqqdejqlv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gpdekxwfo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gincqxwyp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gnjbodnsr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gfseczjwe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gpfqpilib.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/giuiqjuae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/glcgcpkwt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gfoqczsow.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gzwxemddl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gigevbgrj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gevnprent.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gyhwrecbb.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/goknoztyb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gmlwitozo.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gnewvoqzw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gnhlhidny.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gpujxkvls.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gmokhwnsd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gbxyztzek.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/galpzxbyj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gjqfquvlt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/ggxtdujnc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/ghcqriuge.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gbppqqtwh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gwioxwccl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ghfebthpw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gpitieprw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gixeewryp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/greuadoar.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gpvtmywvz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gvsrxakaz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gjldfmigk.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gerlxzeqe.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gqvllgllj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/ggnpzwxvy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ggdbxblde.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gejhexbrn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gswohrjrs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gxyipgyph.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gmnusgifn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gszalzthn.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gibfdyadk.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gyjhxhwqn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gimqltddh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsfvrvsmb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/glnslhtcy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gfqjihnqm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gbdwumqac.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gmhurxcos.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gpjdqbykc.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/guvjwmlsc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gulqkbqud.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gokfsxjjb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gqdqdnxlm.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gxnczkist.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gbsfesjpq.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gmwommxec.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gvwkxifgb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gwwgxgywu.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gddtfegfb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gfqgprbgq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/guniylmxi.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvxjwrrfz.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqkzrooap.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtggojlas.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gocpofaut.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gkwplgxyr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/geapsejuc.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gqivdfesr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gduousjij.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvgjzdvcx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gsnnyefod.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gxaprztjp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/geazuimuw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gcxmkqhpp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gprajqivl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gvwkmimil.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gyaxfipuy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gxqxrvmsl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gsuzgolwu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gjxtmkubi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gtiupokoa.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gjwztahxl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/ggvihxmjz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gwhyznvms.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/ggnpooppb.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gintpewxz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gyfkktbwb.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gevnaggow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gpydxkqvu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/geitqatag.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gnuentmnx.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gxihuatey.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gdwslcpwb.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gpthtcjjl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gfslwcuhd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gczsbwayr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gxzaqdlif.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ghdslutie.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gxibsizdj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gqvlqlofd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/glxulmoqc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gfomufxnw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gdwglytus.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbhgdjmqk.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gtfodtwji.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkognnrvu.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gtapethiw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gocnbulgd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/glivnlsss.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gespmfilb.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gsrmlbxbu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/glvpahnpx.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gdiezzrxy.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gkrljlljm.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gjxpslswq.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gpjtsmsbo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gocqnhsff.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gbxiynwxo.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gvkvkucxq.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gblbtenog.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gibrzbqmr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gqruwdncd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gztowhrkz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gaowgqkog.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gsgbqkrcp.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gdbsemupe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gdlraehjf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gcuylhhyz.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/guuwlrrod.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ggsajgyuu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gmajyocuc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gqovqjfow.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gucywsoje.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gknsywmfh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gesvvydca.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/geofhhdex.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ghzouzkcc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gnpwagouq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gultahaic.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gzygtyyvt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gqlytwagx.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gieksutei.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/guuthlrkv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gjepbpfag.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/geiwknhvt.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gqehdfqlc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gotunyvtc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gtoubciue.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gxzcmrhhv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gsagjlawa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/ggcrhegph.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gyvanekuw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gxlbepenp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/ghjkbarhj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/glbskaxww.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/groeqdbcs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gqfksgptb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gnejzuswj.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gsqbbkbyr.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gieczoeeb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcccidkon.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gbsthnami.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gspwgeqke.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gpdguhqtk.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gtiwggxeq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gogmkmxtm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gcomcqqxq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gtpstqbrr.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gnjucrgxp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gamvgphpt.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gkeegbhkf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gatthoqwi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/goofrnzmt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/ghwhzsunr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gswifupqw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gvsocnlgk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gmbpvrnsz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gamsgtros.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gbqfcqfqv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gppiatzqp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gjgoyapho.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/ggaekjjef.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gkljcccaz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gejobnzex.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gmnmgsmbq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gfazllexd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gitstxojd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/govgomxdo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/goqzsmfjc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/geparjzyc.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gpnvaufsu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gspzaxmkh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtmdqowtl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gnsmuchzk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gpylfgspj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gfzbavvml.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gkduyrnns.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/giqttgfrb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gjmcpvimw.sHtML


<!-- 参考信息 -->