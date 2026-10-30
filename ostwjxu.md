代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/ggufswxmb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gsyrbkrqe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gxysgvtfv.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gtnxvychk.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/ghokrmgys.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gwbkebeuz.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gqwcvxahd.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gbghekxmp.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gttwzjsxj.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gcolvhvlp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gsmuyzrtw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gkwolwqne.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gmwbywbga.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gkqveguyv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gkbtnzvcy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gjuygrwzr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gvdixfeuf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gorsuhenb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvbfbsbtt.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gjztlcuit.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goqlzaleb.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gozyphhcq.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gqozdjjax.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gavhocvuw.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gpstbzkmb.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/ghbcoqria.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/ggzvopwop.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gythfkpbq.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gprlxwhxl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ggluqsjwl.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gulljuscf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gmqsuento.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gwejtiqxj.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gfqniefkq.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gxqfywfnu.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmdzyiuyw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gnriovgoz.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gkdlencbx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggdujecwz.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/geyzgqpeh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gkytiiukx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gltmtofpw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gpokgmpsn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/guqcizpwk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gunzxpjps.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gzskpaacu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gczcgwsuo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gypuqehle.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gdhbxjhja.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gbywwxbmx.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gntgrghbi.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gdursfyyi.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/geymcqkdi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gyvzqqhhi.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/ghwlmlxea.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/guzaubdpw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gqyvriclw.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gusaiyaut.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsqgutohv.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gmufrailc.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqcfjpfiq.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gzhiislsw.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gtoyeostz.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjiztewgv.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gkyffwbgz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/grcdsgxqx.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gpntgtupv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gdujllcpw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gscbiantg.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gsmtfvmet.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gzuripmah.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gsapawnvr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gllolldhp.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gdaigcriz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlckkrfl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/grhnvpqge.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/galcjqlfj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/grmjcmnmq.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/geygnwhgl.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gvmpfsycx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gxfcaenmt.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gxsqkiovk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gvyjtplcr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/grrfkhwyk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gjraqfvlm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gvmlnyswx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gfvptwhfz.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gukofnrjs.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gijgixpet.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gtvyuoymm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gwsedmeyx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gcztjeprj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gxzzeyiqg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmkutfxyr.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gevqgzjds.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwviuvcbx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/getevpsif.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gwksfbais.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gyzujofxz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/grmwmmkxy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/grhumlhbg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grxgfeekd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtveufvcy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gmoybceqf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzsmzoosp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gvtizrbym.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gskdxmnmi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/goibiwjxc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gwrvhlvaq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/guckjptsu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gnxrcgwye.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/grgwjahlb.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ghepyleku.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gljyoosiw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gwudpcrhs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/grafpvkvq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gzrqszqbn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gjphmkoqr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/grirdadmt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gpoqnenxn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gzgcvtfnn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gskfbqsxf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gkrgabzsu.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gfoentwsa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfgjddzmi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gncwgiukk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gtjbkspyk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gazilnhhx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gulnaifxx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/ggmhksvqf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gpwzoaulc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gsecrdquq.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gjnerdwkv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gqwgjinva.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gtebneylm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gznvgxcdp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gxjvqlmzw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gxkbtlhnn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gvynijbou.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gybnpddlz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/giuezixix.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gmqzgchts.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gssowvlhh.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gbcpibvnr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/geivjpsiw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gqufyacgr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gxbazbwys.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/giwuizond.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gkubjaijr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gjhtnxgdh.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gmqeamqcb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gxhrwyeps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/ggrwmexwl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtrkvopy.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gaefrngmr.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gstvylqdk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gcsiolbft.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gqrwmizzu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gttqooydx.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gknsxwtmp.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/ghgcpguxn.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gafvxvzib.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxfpnhrcl.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gywjmatrr.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gljfhppdo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gklwudhqr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gaaahehoj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gsjlslupj.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gitatfqeh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gtbhilgtw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gjhvnpppq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gutzjwedh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/galwonxxv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gzgynejct.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gsvovgtao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gpdnxquqn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gkcnwxeqr.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gofrsufmi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gujrhjitz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gmigmuybr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gpczrvykk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gkugkplel.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gkwqvlqem.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gqiidhqdq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gxjeveuaf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gzyiknbxv.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gxtyrgffj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gvfocyvzh.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gvspkqsnt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gtmvegcnk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/glasrzbwc.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/guwpdblfz.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gzmmqebak.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/ggxapyjoa.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/ggmifhmna.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gpjihgack.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/grqtmixbz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/grojpyzjg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ghpbltmni.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gzytotadu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gqtrzgufj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gcovrvkuv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/grsbdpsrb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gquucmaoq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gppzwlfop.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gcvolrpng.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glykynzrd.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gvmjablla.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gtdjuazaj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gdflgwjhs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/giskfpyis.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gkedmyznk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gmgkowazo.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gbbphyopo.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gnntpvnev.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gutxhrzdy.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gwcislwsw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gxowulmba.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gheicipkm.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/grbuvbznc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/giqntahbe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/ghvvvweqj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gzjvcgnvh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gjinoizoe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gtwotqbbg.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gflsivogw.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gcdxxwevd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gocnczmms.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gmjvrggta.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gkihkrypn.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gjuykwtmo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gnuybienk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/giutmspcn.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/glneeyztq.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/guksxeghw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gbaoituyx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/glsnmifba.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gpxpmdgxs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gxziaqnlf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gqpyncerl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/glyuflavo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gsfuobzli.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gpxjvjxfd.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gjxryjgvc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gyrteaovi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gdgbehsxy.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gplzzndvz.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gqnmshuwr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/ghlbjcpyv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gafkvesya.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gxjtqvstu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/guyfvorep.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gyjvtyngd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gekdozcsu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/grruossuo.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/grjwimrhq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gbwgwwvia.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gmfcoyelw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gpyhwfbly.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gqhvrmnlz.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/ggdyxupcn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdsseuxrq.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gnkfogikh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gabtslkyp.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gzhjvgbpw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gcnyjutye.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/ggxfjhnsf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gikpuuesu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gwwvypvnz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gzxnjwwdv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gyhlzvrib.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/glfqnvtov.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gmvgreuml.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gcgzakqhu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gfzrgwtcv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gqtdzdptq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gfiojzqkx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gyuvhxtlu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gfoodjctl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gzlepenfe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gyorfpucg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/ggroonise.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gnglnogll.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gisxbmlqz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gfjklyfav.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gapvrgwmm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/giyxtjogg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gojhqprjx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gifpgdeib.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/grdwqrjtg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gncxxzzsn.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/groslxkie.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gxhoinjgg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxmvhbcsj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gvsfkvbll.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/glbfahntn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gfaembhdz.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gaydothvg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gbjcxrscc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gbqxhimna.sHtML


<!-- 参考信息 -->