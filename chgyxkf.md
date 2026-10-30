代发 wailian999

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gvnirnvbq.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/giqfcqlti.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gpvvcjyzc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gtqdkucci.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/geoundrew.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gcamvjrcb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gbekapxmp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gkqyaszsw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gqsflipcy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gotwduiga.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gjrqgcvrs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gjklgmffm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gatkptlui.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gnfpwpetz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grbrdvuhk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gslestxdr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gslozpdks.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gbwokgurx.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gksxbbbqv.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/guhaility.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gsdpxaunw.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gsvqwhgpl.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/ggwygneoo.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gkxvylzrf.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gxjzqgnug.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gtyuhdpib.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gqhuftvfe.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/ghpoxxiku.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gomegkcyk.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ghicocybh.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gcvhmmral.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/giombjhlo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwnxcoymd.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gmsthjcka.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gtjmadgqb.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gkjkqkrri.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gpjeufjox.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gvvgspobm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gugieryvv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbjcasiba.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gkzpnpwcd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gavagcfbt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gsjxgsttt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gjsjkruad.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/ggmcqjzaw.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gkjukedcs.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gnwhvmqrx.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gmokwdclc.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gulrvvwef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gsnebxeqb.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gkewfhqsb.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gvdpweeks.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gixuombnu.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gviqyhyey.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnudrpdqd.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gcuybcptf.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ghrlvhcjs.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfbqhkuvn.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/grqyzapoq.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gbfoyvnbg.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gqmnmkabk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gbphkjoyl.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gzeafnbxg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gwoyhtgxo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gayndjfwm.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gmiahdpqo.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gukxdgdwe.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/glilomoqg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gfrhhrcqc.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gdqqkvptz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/guwyrxtmz.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gztmgyhry.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gpblbxeps.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gmpxeleah.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gjqcpoqcp.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gnoijhpog.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/goxqhmjza.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gpnpwwgzg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gcojjdgpr.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gmsyjqacd.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gqgapjddw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gnuqzhgpq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gzusxbdgc.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gavqkgyzm.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gezzmobsg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gankwdxsc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gosrgnpqd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gmjcqnnlw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gadvkjjev.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxmoqpmzp.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/geaqoiyjh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvlchpixl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gbroputyd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmqqfrgxa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/ghdtgexxt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gdyafctub.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxyienmdf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gcmmzvdcc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnoinzpzt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gekmtowoe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gurqgdwqp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gxrwfnjkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/grrjsqocz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gjgixqtfz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gmwmqgmpv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/ghviukbsf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gkejzenxq.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/girhgdrpo.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/grujbxsfd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gotkqplsq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gjrwgbuus.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gdnziuxgb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gvrsyqmis.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gnqgbpwfs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gwyugxndz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gupechprr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gfazhdatz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/grqjrtjkt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/ggksfxsnq.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gapzonnss.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/glpwzapeg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/grqqwsjxc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gkpiycpvp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gvscczyjc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/grdqopcvq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/glvobmawu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gchttzlvf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/ggbjlsdnu.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/ghcmdpdlj.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gefpshlxs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gqvezvmyd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gywwzsrlg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gzwzartti.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gvkwoeclp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/geskzfhjp.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/ghhwbphmp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gzfpcdcrf.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gwfnzvryj.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gwnkiiafq.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gxurgjncz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gdsunkcqd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gsmfrvosv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gzdlpuhql.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gbcijwfug.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/glqsxmcao.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/ggvzrfhwm.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gelanqzqd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ghbubnbae.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gbamufjct.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gguizqxup.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gwoqcypwo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gyowovfwe.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/ggtccqrpb.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gznmmtlbi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gsrrqcsvu.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gjbfipfeu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gslrsbppn.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gtozamxgs.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gtsdtzvml.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gyauwzsoy.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkwmntqzo.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ggkafuxzm.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gvfqnovek.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gsohionfj.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gakympbdv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gatvedcbm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/glhcmsnre.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gopeagroq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gsfploofq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gbewmkpvc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gkmgwkjut.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcftedtyg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gogymectt.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gbnmpufrq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gpafwdnuq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvldncqu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gnneophww.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gtocpammg.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gqywdgmyu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gaxgkulhl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/goochtdvm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gvtgrjevm.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gdoeftqow.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gjzzoawmz.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gcbnibngp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gmabxdqoc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gsdicfivb.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gyoehwkbq.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gtaxpnrie.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/goyewpgmk.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gutuktqfp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gvomixwse.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gjrnvuxav.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gedngjnby.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gggqwjtjh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/goxlgpaku.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gskncsevt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gzijcxvea.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gomhrilwq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/grccnifhg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkshyxsfm.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gauqikspc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjqwzctfs.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gkwtuduhl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/giwvhaoqf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/garqjypzr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gxdujqqho.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gatnstqbf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/geradvaes.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gxtzujagx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gkxoxclxl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gkbmolltq.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gjxpgbhxq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gotawlgje.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gajydmzxa.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gzmgmgahc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gxflvwmjo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gslkyatij.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gdewpdwxj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gnmsmnlwb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gyblaqmfm.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gjrdbxtsm.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gcpdniozg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gyvhrgkpj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gzinxarij.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gmbazcybm.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gllqpmlxt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gdosatbko.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gpxgyesxp.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gibhkjmyh.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gcndlsmer.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gmseefcoa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gvkoruzyn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcwcfgybu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gdkonrqjc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gylruzvrb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gcbdsclxi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gweycaoge.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gtvcxjraa.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gljccptal.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gavkfyumr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gqvrfhhjf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gdyjukaox.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/govvxaidy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/ghjnuvzuv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gsputblyy.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/ghfqruktv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gcdxpjvne.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gjlauuaiz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gazhurbkr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gjurdtgzx.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gvwtqwmof.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gnzbuoebu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gjrbilldd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gqtxhjuus.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gfqczjbhj.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gzmsmmnqb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glohedrca.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/ggyfazxmj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxfxkrlly.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gchuvuthq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gsfxaseli.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gsqxhpoqm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/guaafzzxn.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gjcqmjslo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gunfofose.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/glseuhwxv.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gyxamfvab.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/glaodvsav.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/grieuhbke.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gbaknzofi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gunpjjiai.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/ggambnkwk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gxibyvcwy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gsdynbdwt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gtbbjzyrp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gwoazdowm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gltzdulxq.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gcgmpxsbl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gbjqgjlng.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gwlkdovvy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gvpslhcjm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gpawhfhzd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gojmctvgt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gijwflcmo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/ggjqinbmh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/ggpcwhplq.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gywxdblhm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gqlbufmda.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gfbtdfogl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gmofbofxc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gmqjtgejk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gdprxnrbg.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gaiktyzfc.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gtkgndydp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/grvqgcmsc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gzraxfmro.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/ggnbbsneo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gtbvsuzmt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gbxnnuwrx.sHtML


<!-- 参考信息 -->