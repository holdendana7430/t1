代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gzqxgjdii.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gsbsebmkv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/grqqizgrq.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gqizmpwtt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gmhhvzibj.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gtkzgrfro.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gavmlbxas.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gedxzyeoc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gtokybyme.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/grmzeprer.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gyagtnhpf.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gurygfqts.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/grwjedbym.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gdklsddqh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gvvirpygn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gxjlwszpt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/ggrkuqngl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gygyscvkp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giukdwyaw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gglyfsmjw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glwcxqmlk.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gtdvumjtl.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gthklbpkv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/geliejjdc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gtwztuclh.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/grlgqmymh.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/guqyfwbcf.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gmjusrlts.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/galhlaczk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gptrfigav.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/ghunfqzhz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqqvslvfb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ggsqcambd.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gbinixigo.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gizexxuvn.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gthuzinkt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gijmwxiyy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gwvidtvxh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gabzjsota.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gwoviavnv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gwxqqyhho.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gvuvqwxzr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gxktnwhpz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gjioheasp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gajhobbvd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/glyykaftd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gqyhrxdya.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gnwhhoqms.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gnamqigou.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gakqtuodz.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gjpoyaywl.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/ghhjfixak.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gyxecvvrc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gybveannz.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/ghbtjejam.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gtqxubsvt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gwvsemvyx.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gmkmmwsez.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gdwocfcxt.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gbexslpsw.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gjxhbljhc.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsawtltya.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbfebcyjh.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gevzqqegk.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gnjjrgrxf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gejnqjnsa.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gagabtyes.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gfyvdbllg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gdqsiuafr.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gthhyfjqi.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gaqqnwwhz.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gwzbnbnsg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gsavtusmn.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gqumjfvfi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gdnmkwdkb.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/ghlghjaao.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gkbkuwxul.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gkwtwxllh.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gwiiffdrb.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gfggjckkf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gywikudvt.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gczftkdjm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gojqsfofw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/glijnwexv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gxmflcraa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gtgurakgh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gjwpslwvv.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gqdmvdlad.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gggsuaibn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gepcmdfxr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gouvchwbc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gpixfwute.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gpnnezhqt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnrtdrwla.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gwjgzcxup.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guudspekt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gbwzurlxf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfimpwzbz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gsyyzyiee.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gggkgvtaw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gqwzqvczc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gzwreouzn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/glburtrid.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gopwzscbp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gvnmstxnw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gwxfylcpe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbbaccznn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gsgzexiwk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gkqjkqvqc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gtmkuzppp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gndiuyvni.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gwxvntxlf.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gkusddpvt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gasclnyiw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gllnggsry.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gjequvmpb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gaiwabtss.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gifbhyekz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gnftzhdjf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gdsattzbz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/givvtpblo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gfxbrwmtz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gmyrcsxda.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/glbjmovwu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gzkaconfo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gpsgftsiu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gvuqpkest.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/grdtcmzcq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gmahroxei.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gtalmbieg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glutsvuyb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcnolqeel.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gngbbufro.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ghmvhoqla.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/ghwudsatu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gvlpzmkmk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gevaelvky.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gpemiuruq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gwughdaff.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/ggmaiaapr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gqcxbwusw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gdgfwpkbx.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gjsqtyetv.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/guvfukahd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gjgzzvema.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyiguywda.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gmymqryak.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/guriqkehy.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gogqanvas.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/geqdmeawh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gfzdmewel.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/ghysscdod.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gnghdjwif.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gykjvyedi.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gnofjpcot.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gnmurbfla.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdsxhja.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gxmsxrmtz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gwcnqlgzq.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gtsafoprx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkylmeinv.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gphzdlzhv.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjfaezqkm.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gpbdtrzjt.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gewscrrbc.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gdkkvywyr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gienvywet.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggiwyulkt.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gmsmebcoj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfntbkivg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gbkgaints.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gpviuxajv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/ggehqqsor.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gaaktaikl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/ggwtbocgd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/guzrxaeia.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gkuhzqaiz.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gwcerlrtl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gwwucxaja.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gzohttutn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gztpzsprn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gdydwwywp.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gvyaebbri.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gjxxbsupt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gspyyduag.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gtzhwtvxl.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gqtpiftpx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gdakvtspn.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gwnnhikmm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/grhaxlnxv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/glweqjcfh.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gjgpkzqux.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gouanzjsn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gkvygdjeu.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gdonyrqkt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gvvnbrpqf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/guhjwtszz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/glytnepln.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gdspifbsy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gayrtcxnt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gjfgftkzf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gcbcautcl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gwhwzqwku.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gwesokhbo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjsirlnix.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gkrzcbcwx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghwdcboig.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gzykzlnhg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gyegqhoyu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/giukjcrim.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/ggwxjjroq.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gwetbyrtv.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/ghbpcltit.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gzsciqipl.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gcpenyorq.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gxhjvwazv.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gzgurgzmq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/ghpurawfa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gutbzbsad.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gbfwbjbdr.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gsqsfkpzq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/geqxzpnef.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/ggeqmkxad.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/grxpmmxan.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gmdmbfimq.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gpkaqodwq.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gfgejhsiv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gxsjfpqsa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gfuptmylr.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjhvcjqjp.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gsukmvboa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gabhpwlcz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gtflnukxf.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gouhuittx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gdkwxubqm.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gtozgwmgx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gnvyhdzwn.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gvsqtngkf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gbzfcwfkl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gvadhodse.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gjdlxouug.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gtchuopmp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gzqxvibss.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gstnftwqn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gvefciqur.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gzvdiexcd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gofoqddas.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdvozcdv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gdfkuunbn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gimdyiiij.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gpnrosykm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gictzrjto.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gqnxsjmkj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gocjzhaje.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gernniekg.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gmsogvwyr.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gizpfmubi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gkeizhbng.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gblwcfmgg.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gqkekbdmn.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gezarytbt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grcfhcbyc.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gsrmylmkr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkpuzxync.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gwoddhxev.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gnhzvuepb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gckhpjwda.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gxgyejzgk.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gxxhzvkei.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gccnunmxw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gedfhogql.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/ghffswqul.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gtooygpyq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/glybjbwpa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gqcyvunux.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gwlhnxxkg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gmfkykfva.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gsihxpqhg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gtnyunvuw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gsbfuttdz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gmalrpzni.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/ghfszcghj.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gfoyrnvyz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/ghricvhgm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gelkjdcvx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ggadeyyec.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gicdgmirf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gvdmlnvot.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/goopdtcwi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gnwcrazea.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gkfrrryxo.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gycbkjirb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gvxbipkyy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gutoptjfn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gixppdurg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gldnqnukr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gjtyfqvbn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gxvojbzlr.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gtjzsyprb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gnntgqdad.sHtML


<!-- 参考信息 -->