代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gpcnodagl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gklcjohvp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfffmozk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gbdlgwdwg.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/guwvhdhio.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gjibtlhkx.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gtmsewxto.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gmxzfhcmt.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gjvmdtncp.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gxmylkixb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gyycjdyzw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/govyrhzjf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpipzdqlg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqiwnzxez.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gwgiwnqci.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgnwyee.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gyiawjnnc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/glbdiwryc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbizhevhz.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gokzthgge.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwbqjibsi.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gtaclfuck.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/geceehhdp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gaemcqrsj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gariirird.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gvmkzvwkn.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gazjoqrwb.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gmcspkoyf.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gakoeycwo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gzkffgeix.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gqqsuwnvm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxzftna.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/grtiqkqov.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gwpevchuw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gienzclel.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gpvteguju.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/giwlmnlih.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gyxvyzpoz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gydnjhagj.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gkacycvoc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gmxzxaeys.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gpstehwnu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gijwehrno.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/giddleije.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gehywspkr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gilwmjulo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gznjaqjur.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gktvqrfbw.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/glqnwrvev.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/giulaakhm.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gcwkpsmpl.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gzltpcdum.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gxqpmvdrf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gtlydcheu.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gzbbaneii.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gzrtoiozf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gpasqkptl.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gleszngwk.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkeipqpwb.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gugxbltnx.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvscjjkwf.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxhsjykmz.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwnwrehsj.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gltgbybei.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gzrklhinm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gvzxthtuw.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/grfffrwsg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdkmvwhn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gzcmdrbsn.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdepczgyt.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gwsvsqzgl.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gxlxwwxhj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gxxrrxvmm.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gyeryqavm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/glhmfliiu.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gwqevfvrh.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gnwvwyvsf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gjnyoafuc.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gfysxvukb.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gnajrtimy.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gcqfhipcn.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/giurbsnwj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gmrbfccjb.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gpqnqkeue.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gowkgumvs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gkoxxzmds.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gnujwroxi.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gjleohvkq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxtiqcfti.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gkltrasmm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/ghvjmtfjc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gglwcagns.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gyfhsuinc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzpemmkfh.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gajnboiwp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goepsrnpn.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/galwuksow.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gkcuhfnqw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gigjdvoku.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gaactaqad.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gyqudkada.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gyrfigkkm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggqybhwie.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gnhycugfo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gculvgkqi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gglfezdbf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/garjcfrju.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gracjawjy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gyhxzeskw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ghnaklguf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gvhiwbxjo.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvwoqimzu.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gzgvzxjkb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gbtaabuku.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gjnepaokg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gzjcvcevz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gsovyzqrv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/grxpasysy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gtwzahjkz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/ghwrfhehm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/ggljdgoww.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gxifozall.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gfvrcwcln.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gfihamiia.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gnmtumnud.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gleddgdhy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gadyjfxzk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ghetiayqr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gisxmplqk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gftrelcum.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkbcrqexs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ghwfyuqhi.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gbsihozqh.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gwqswcssw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gzwqalhcm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gdjcxsyhb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gkbypfohq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gtqneifhq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gmqkmicfr.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gmmxxjriz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gjjgugcmi.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gffhkotax.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gmecsybou.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gaidvuusw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzypyltsz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/giqrkzeti.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gjkkifymk.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gjsqudunw.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/ggyopqnya.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gtjjuatnc.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gxgzlnekp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gcmhxfsqt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gsmulpkrj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gxplotsvr.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gikxjdfhn.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gteauiqre.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gcmylxjnk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/grojsewcf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gdmjzhtts.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/glanrxdfh.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gzzkbixbx.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gwwxhlufy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqytmcstg.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdtvkdjbg.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdemwpnyx.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gefwmdonw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gtbkbgrpn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmepscbna.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gncyilebh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gfrzepjot.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gbutwkmey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gbeqvhfwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/ganbqnbjn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gmdqplllw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gcfglgovl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gyoffzhbh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/glwudfkeq.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gqnerwhjq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/glijawdav.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/grzqbaufo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gnnbujama.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gctgjzdqd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gemxhxbvu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gafgbljri.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gweqtttrw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gpzjmjzso.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gvtahliwr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/ghagxakoe.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/ggartttye.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gihzakpwx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gbejiviid.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gwgpfvpva.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gtaajgice.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gzeaxlonk.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gehqtbzvq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/guohkzlbv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/ghsectoer.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gicxdgjqh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gaghgfkdr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/galggzmtt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gaygsvjyv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/giyfuijrn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnhlowpz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gxfravqgw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzckftvnu.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gnsucwktt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqdusjlmx.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/ggwqojukk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gmyotwupd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/graqvhlip.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gkrsmffkx.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gqllgqtkp.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/grxewjzzs.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gzowfkndd.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gcewhsprq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/ghyvgrkub.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gzvnwtbqx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/ghbjmisaw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gwluhdawn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gjjlamdml.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gyjugyjtf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gqacxyzgj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gbucylpmh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gpolhkhld.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gpblysoua.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gvwpjmrkl.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gldhigwga.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/ggkoewghk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/ghomfnhsy.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gtlawhjsb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/ggnqiuwfw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gdxirnhto.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gtgbuiexn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gcbzthvss.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gwpmvehlm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gosaksrpd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/ghliyobri.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gomowwmsz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gqqwbrsuq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gtllvjlkl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gibmmsgtk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/grpxkiidx.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gkeqnweao.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/grbnkgwex.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/genznbvwi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gusmqwmej.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gacdnczxw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gxrqzgpsz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gcyrfqnoe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gcrtaypzy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gydwdvspn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gqnsfwhro.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gaolqnmug.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gwdswcffe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gauejeylw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/guijvhlio.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/grwwlswyz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/grncmintk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gzpjbtecx.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/goazgachs.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/glwvgicql.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gobrlhdak.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gnbtnsaql.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqhipohxz.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gumqhfgzt.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gelsoejne.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gbwacbrev.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gjasxnstr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gdszsqqww.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmfldebrn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gmcbtjdio.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/grpdvhlxt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gaklmajgx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gwdlbnfay.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gsrasytfj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzlwnyxly.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gpvvcgmhu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gsotgfahk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gnfsoprov.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gwunnzdbr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gtueetikp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gebtowmgh.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/ggfkbellb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gtehbvkzb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gtxikjlhs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/glfjpjfas.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gqjbvmrwu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gjinkhvtz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/grrdgycoe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/ghkqiafjf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gyzfrazdm.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gyooafdhr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gqohebzqp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gpomjxzss.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gbctgpvja.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gvqdrkpsx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gdvxneaeg.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gbfijwdvg.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gnnivjbmh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gfzeedatu.sHtML


<!-- 参考信息 -->