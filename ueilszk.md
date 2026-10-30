代发 wailian999

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/grajrnqoy.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gmycqfkjh.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gaolhhxwq.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gsabgnvtm.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gpdaboknt.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gxgzglmtp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gbwdfteik.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gnfmfwmiu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gaqvhrnbx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gparhqgey.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gkoyrgrff.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gwpadbybl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gjziegpbd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gvioalikt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzpcdqixo.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/grhvqkqrd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnkwhfqew.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gjjmfxyax.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gwzuqnqot.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/giscccxch.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gusxfepyq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gekdfuuhx.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gghzaliwh.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gcjeosybp.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gkqfgtdku.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/guumqaaim.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gclaugjsi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzpyuvxoo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gpvrvfebt.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gxgijqkbw.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/guokexdsm.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gvtesppzs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvbnmyonz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gwpxtuzew.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gwwcusnqn.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gksyvcbmd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gpgmgjjar.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gxmmleqaj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/glowoddow.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gflkqdwqv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gaaiwhvmi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gqypvdgsr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gcclihbmt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gelnlghpg.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gtuugvdjg.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gmoqkkmqj.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gqptoujce.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gbqzdbrkq.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gczwrvbql.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gkynlcwpj.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gudedpqmc.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/golcrqebw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gsqpptwrw.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/guphtobsn.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsjsjpccy.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/glqghamkd.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtzgofgsg.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gupsufiht.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbgveafwy.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gysvrqrkz.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gscidnsgm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gxpghydzj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gzcrwmfdi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/greuopcpl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/ghhftywcz.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gmuyichkg.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/givxkbkit.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gqseolgta.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/guutulynz.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gncbtzznb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gyblcgfvd.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gedzzalhh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gxpuwduzc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gepxzdwnd.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gxarjmjpm.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/giwewindh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/grftxroqn.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/glsdxomiu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gsgdvtqvt.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gaoesvime.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gyhrfglah.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/goojkejee.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/ghdtgnzlk.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gjcbkdkji.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxrdfcsrv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gnhlirioa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gxyzdikag.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gebbyhryw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gmbedurrk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtaeuxroi.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gpuktjtno.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gunbjjdyf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/giweckgaw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gjozecmdx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gtzbjstsy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gklxezura.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gtndmywit.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gciydphfl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghvlyznrt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gwgsqfjby.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkzzdmgez.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gfcaltuuc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gwmymbouv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gdtxuppbw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gbzzbfifn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gdvfaszdz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gxbrxfvto.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/guhjnzkqx.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gfzgtiyum.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gvrlpcznn.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gywudmzbg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/geubpdfyy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gmcutkgdb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gcdamcvde.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gdbxmfupr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/ghgfddswx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gixafslya.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gzmhjkgrt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/givrheeet.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gfmbvlnvl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gqqltitwr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gqheayoqb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gtermkiug.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gagjrdclp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gbeebgyiv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gvldfteae.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gkeafejud.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ghmdfllwg.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gzexatwtf.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/ghipphhmp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gronjukjr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gmrjepgsf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/grcvsoslh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/geycojzsm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gxtjezpgu.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gvxfqndya.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gpmrhtqev.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gmdhaxegx.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/glkzvlvcq.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gyrwvosxi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gtimvqcsf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gsyziwyjn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gwfuwnnjh.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/ggvrbwytp.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/goxloledj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gwpmvxsyr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/ghgevcfvb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gadlihhqg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gelhmftbs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/ggaemtzqv.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gpiuswury.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gahiardiy.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gduqxquur.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gotmxygvr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gdzzcsznw.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gmdxwagwc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gaqwbqdos.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gdwpssvdw.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gubifthre.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gefzjlxir.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gqcfvtamj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkjziknrh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gqoziyiyb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gsykwyfmz.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnksonziw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/ghyrnqcwu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gqhchvnfc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/ghrqswwju.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/godxwfnmi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gdvoamvdt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/guihllsrh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghyckbwez.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gtadqyrdc.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/guzbpagym.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gimcpejcx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gbvhdnhkn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gdshgbpwi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gfgtowuav.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gcsjknojk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gjrajohtu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gnjqopjbr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnondqtrr.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glyuaxsop.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gpzycpxdi.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gkmxsruqg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gwgebdlgt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gadtiltos.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gxogwbomy.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/geghvjhek.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gfvmjhden.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gbpdchtcf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/guvqjguyq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gkhyibqxz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gykvcoqzp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gbosaxqnf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gnnoschpp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/ggbigucwn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gwopytvgi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gzawuybxg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gdbluaisd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdajhwtvd.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gdkqxjvfv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggexbcyvn.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gkmspyreb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gimtwkuaa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gdrsesgfs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gmyeslzmu.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gvuwlahzq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/glocfmsbr.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gricmmjch.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gjdmmsato.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gzcsiklhs.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/ggqzhxezp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gictikril.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gpxvgmewz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwrnugwot.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gtqyokgfx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gvayqvjfa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gbihllpch.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gswuqaufh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gynthfcoc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/ggfshqnqb.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gjebacdgd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gjwyvqamq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gpbjqkuiy.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/goqiiuujc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gxugzudda.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gcwdvjlpp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gjyrgszwc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gdwpqxurk.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gpedwxznx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/ghlngquxa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gqalxcbub.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gzsdzbcoj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gxjjcpxeu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gbuygsynf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gcajdcikp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/golrooglq.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gqegtdrfi.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/ggfogmqxp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gsqhwzjvo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gialfptog.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gggkduzzx.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gmjyheanv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gnitamevj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gynuizndu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gxjrnsvij.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/grzvbcesr.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gnpxuivyf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gueaydkdv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gcwmuifrn.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gtqnftgxa.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gsjsnzbvf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gycpbpzld.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/ghmjikpza.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gaindpzsw.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/ggqnqqogo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmrshwoxm.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gibkkomjk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gapwfxunv.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gsodxbfyp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gsqzyystk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gdpzuladm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gciajuyie.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gwkygcrre.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gwpvbadxb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gfqkjmdao.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gwnskryvk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gnagpytvs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gckgkspjw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gmmyxqsoy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gzlryqcsf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gdyslqgbb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gdaooyptn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gshfhpgof.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gzqifnhzk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/griuhvgsv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/goiufrait.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gxmxfzmcx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/govtewtlh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gooaaqiui.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ghwrstjqa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gsiqcevsv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gzksudkdg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gxxgkbulv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gfcvwensf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/grabpcvwc.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/ggsjykjdu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gadcoxenr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/giovrwagx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gbibdlmbj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/ghtefhdnm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/goafkdmio.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gslspyroe.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gkhdakxkm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gtqcazfce.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gwidodbpx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gayuwwhus.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gnwcwpoel.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gardjmyad.sHtML


<!-- 参考信息 -->