代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gnoslcavw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gwdjvlhhl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gqgoaoxch.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gommmrtgz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gzloqiqut.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gahudkkha.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gxpnpzntl.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gikzdhtbb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gijtgdcca.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gnjrxiwrz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gyalffcho.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/glhoelxou.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gckasmzef.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gwdcobywv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/glxjdlnev.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/guxrpnhwp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gpolcpecs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gxiprtwtp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gphtfgfle.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gswhpheli.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghatktwfu.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gqilgjyjd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gfitggjiz.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gqtesuufh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gvihhyepi.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gfydaseog.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gjgwsuses.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gayynazba.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gxsxnelda.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gxcdxbyzt.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gamhimmhq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gdsmkgran.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/galvrdrhp.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grkstnsgu.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gpoexjzja.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gldcjwcrz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gzrchseew.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gdtjbwlzu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/ggghjpuhj.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gakadvxaf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gqhooewbx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gjmefqgps.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gefzuowdd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmymdczxh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gsvvosudx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/ghngzpzav.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gosfnblcv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gnoslmebg.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/godaqfcda.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxqczuwwh.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gsolqukbb.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gizxjqtzi.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gegltkjbs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gtyssstwg.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gxknqeyso.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gwjhxrvgm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/griafonpf.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gzroqzbee.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggdbgtkxo.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gggfczehh.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gykzxrhwo.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gaifzhdla.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gffehxadz.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gptitamej.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/goxjvrtmi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gosqfvkzt.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/goiofugqe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gobqkgykg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gobfnsmah.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gjegxeqsa.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gbmnowsus.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gvwqxjpky.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gwvyizapt.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gmlvtgdgr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gsbofjtgh.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gfoezrgpc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/ghrdwzdtu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/glvjnwwla.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gjwpknhme.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gplbllpvx.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gownyftfu.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/ggpivendq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gicwacvow.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/ggpivhgme.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/glyihfwym.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbpgeus.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gglbriucx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/golrvaeof.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gdcepgbgz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gqgcphjkx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gcjekbxli.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gowpdvtye.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gvrupizjg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvfssqieu.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gvacbbpph.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzaygycnx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gmdjsgxbl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxiaxcffo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gvtixmyyq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gcorxapny.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gfqzayhmp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkabtkavt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grkebhbkz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gogpyjywj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grzvrjqel.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gyctbvtdb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjvernxsi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gjwiacrtu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gijmksixo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glnxxjqze.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gtzfnixxy.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gurhtrjvv.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/ganygdaff.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gjulucqmw.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/goztvjswv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gjfqtpoxv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gtrsnulrn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gnpmbfkmp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gutuqzilh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gqwdeuzke.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gelkxzvhg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gnyrlfybc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gnmqpqxos.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gmipkhrxr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gkcqergzm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gdskpfshl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gzsviaejg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdeqhnnyx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/goojytrnt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gjbbcaphx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/galapqcqw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gkaqxjfou.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gsbbjtxnp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gqupgzhan.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gonrchpyj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gjrsqeibq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/glkeulsfs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/ghjeohzim.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gxrmfsbpq.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gquirztsv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gxyxydcwr.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gccmbuhpg.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gihcxrtvc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gfiefxcvb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gqestbkbe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gfnnpaann.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gpiayuvvx.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gtnbehmdd.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gipcitkko.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gowqdrncz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gwcmumkre.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gpvtnllpn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gzmxpttuv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gmxeivvjp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gvuwoznox.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ggiurzmys.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gstgvxjwf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/girpireor.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gotyzrtlf.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gexkrwzjs.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gbamuetjg.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gjxgqakqy.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gplnxergu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gaskhwpjt.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/galxomvhb.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwffeimnj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gqmamufcj.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/givfxpqsa.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gkishibtg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/glaitxuoc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gulgwwzey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gwwjvflrn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gwsibjwny.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gfsmuyhym.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gbbdnsfxm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/giklinvly.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gxfyrqdtf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/giyayyamu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gfbonwhvg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/ggtxrwrlu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gcabkpazu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gyvkmzqjh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gaszfvwlj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gayfcyqlj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gubvkeaxx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/grswgwxnp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gucotcxld.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gtdpznvci.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gbjelaxyf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/ghgsnwlzf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ggefmwwvv.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gyphjztvc.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gftllwxrq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gkmaoeqdm.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gdfuikblg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gzjcfgrbp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/glpruccia.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gtssiyduj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gwedeugkd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gojysgofy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/grgugdssw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gxqbnrljp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gybflwdbw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gdimtoqku.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjipvacps.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gyvaayilq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkxrrxnrv.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gqlajunxj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gnguobykz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gxglygivh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gwsuyhfxu.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gpoqdrekh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gurzghhvb.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gggolurba.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gmywaztxd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gjdrmmmua.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/ggzasvokf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gmyyebuok.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gpvafwwqa.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gqvbycfzm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gxeejhxnt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gyjvalogj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gfucxvvvc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gqfeiyhna.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gjudsoijj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/ggxjtflmh.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gtquzkogy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/grawpsqfb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gunuimlyy.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gbtfsgrbu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/ggdbekdye.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gxqldiaso.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/geqtssvjy.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gqmxkxzip.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gektodxtu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gqbzfzpnp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gkxtzugwa.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gkrrkouut.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gqzctdmwu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gkzrnqhfb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gtezqtauw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gxtlatrfa.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gvyxmnbwi.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gbbucgyrz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsxcdjjy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gzknpiwzr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gwbrcjtkq.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gqzzlrlps.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gekebaxlh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gqiztpbwv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/ghupgqxgo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gccyynjfc.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/grkyzosww.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gruolkvlj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/geuucickt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gyretozdk.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/glbfwxhpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/ggyyyntzh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gtxnvkzpy.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/goinoajcn.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gtnonjjfr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkwcfhyjz.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gdbxcfbye.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gseytibvr.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gquzewvse.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gqgseammk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gdsfihruo.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/guwrdztqa.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gngwxzgqi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gjnmntzcc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gmnxgbswa.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/ghvzgtujo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gezlqpzhr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/glksrywyn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/ghifamhxl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gveydcxpe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gguodmltt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/ggalxscrd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gkckgoamn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gjtnuqnvp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gwtiycpsn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gihsdvjpy.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gesocevxm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gugnjbgug.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gpvztwmem.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmbzkpgyf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwxlzbkk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gurcrzrqi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gzcoaooqp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gipymaemi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gvyvfqsvs.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gdfmdgfwr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gpkkdtprz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gfecyfsqe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gimfwfepb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gtoiioquo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gfomcrlwc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/guzpgymnt.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gcqfmckpn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gtyxlednk.sHtML


<!-- 参考信息 -->