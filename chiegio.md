代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/grjekxlud.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gdawbwpqv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gjnntsgmc.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gaejrhovo.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/grpxqarwe.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gnslwvtjj.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gdryoowvw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/givqjrywl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gwrxdlhbp.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gqhfpgwtl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gxuaojznj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gehtpgysw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ggmwtzcsm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/grfoddnlo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gpkzddmmk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gzbalgzzk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gcolwblva.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gcsbkbwdf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guizdicgu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gknpdxlfe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvhicdcwy.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/ggfahujgv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gwsfinomj.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gueuwflks.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gvfrakhea.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/goirvewcx.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gezmqtgeh.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gumrbkadt.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gkstphloo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gbucnubbp.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gpvmkpapm.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gxguzyctu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gaefjmdgc.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gkeofawmz.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gsbrettrw.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwpjtfwmk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ggruyggff.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/ghezuddkx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gxfemeoqr.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gfmpneguf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gqqlskpoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/ggitpwgrk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gzkqwgdqj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gczzriarb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gxonmkags.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gakevjqkn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gmjdovlgd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gtujahina.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/grkbbhxoi.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gookjuigc.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/geauervsd.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gpjlqsvbw.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/goxttmabx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/geucwjxsp.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/ghyaxhlgj.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gomqgytui.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gkmonfpjo.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gwvtvdstm.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/grmmuwsvm.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gqevdtyob.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gckwcnjbr.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwbnolslu.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwrfkuvhr.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gwiipnrhs.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gijcstejz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gvxykgueo.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gqyomyzbs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gqnwxjkho.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gpbcsiozg.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gjgzegcfi.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gnsdlitbm.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzyqnmmjy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gvbbuekvx.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gbcackeyv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gqofyhjtx.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/ggnavpvre.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/ggjhgdmck.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/grlxvjrvb.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gplspqbrr.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gcrejxfeb.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gmadtzyho.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gmjkeeqxg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gmelctpkl.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gzhdlydlx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gqwbbrkqj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gllmgcgwb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gkdxdvllz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/geycoayco.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gjxyoltgf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gcnyqriup.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/goxhwmzuv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gldiunplk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gggnabcii.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guplwuhdl.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gzdgjlpuh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gslbscere.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gkpjjvfom.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzgmbkavy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxtbwxftj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gexfhtsqp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gryzgtpbx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/grxynecnd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwapajanm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gxewmirqq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gydlcfodl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gbgsyyvdm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gwsyfkcxm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gpupmoiws.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gunwsqmnj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gmvjigiuq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gxmwkdvyl.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gzchdvtbp.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gzojfuqab.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/grnhxzoat.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gsuyhxkvm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gruclgjft.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gqkuxfdno.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gnqqdmfue.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/ggmsnxpzk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gjzezylzj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gviegcrsd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gxwjlfinc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gskpfqlzq.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/grkuutdrq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gmdjcquww.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gqnhlqqjy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gjyjgwopl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gqhdyupje.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gvrxortbx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gugdwqevn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/giebtwntn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gtcgrdihu.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gogucnwxl.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gtemsefhm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gfdxckmuo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gtfqbgpib.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gkocdirri.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gevqgaieu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/giheigedo.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gindfqclc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gmlgpwzud.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnkfxwaqi.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gkyhmrezb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gclppxxbm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gvehswwgs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwjlqrrgt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gfiizisap.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gnhcvnewj.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/geucrktev.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gpdnyrsxy.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gilhnnwuq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gjgfxirab.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gcvzmnfho.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gmutunbqh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/ggnwcdxnb.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gbjxlxzlx.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gczctcjlr.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/geesbtcwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gngaingcq.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/grhuglxvw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gndoicvkz.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gerpahssy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmjeerdhm.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gxicehrkm.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ggsxdcwbl.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gyfbodzih.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gwuytecyu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsrgsfmqt.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gxnmezgzl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gaymzhowy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ggumzbvdk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gocaftfmr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gmmnziwva.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/glnhboezo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/ggktjnwae.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gnlzzgozy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/geduvnaxf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbnlieo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gapvmwlrk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/ghlgwckya.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/ggyolqkqb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gmsgcnnvx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/ggwvogczt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/grfubnoiw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gchzjzasq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gcsatggko.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gcbmbdiso.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gpcwgsxao.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/guhumkorr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gcjspjjwl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/glbbalopn.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gtoxjpggz.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gizvxkhtz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gjsmlkgtv.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gilrtdwqo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gejnodmmp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gevwhndrb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gbaxjckxe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gwbeioweg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gfcvwqwhv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gewwtpdff.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gcxlbrraq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gbbsifcnt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gcuamvwhm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqabimqvn.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gqirttsqx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkaadpnes.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gwoicfguu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gyyqywweh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gcylmatjp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gwuheyhrz.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwgjskcuf.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gsksfzqgy.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gunptspes.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gdexvtyuw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gsercuntn.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gcuvpdebg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gvilgtjnw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gtfycadfz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/glmvdfkgv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gndiiburd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gsiirwguv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gcpoifcap.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/ghyosqfsh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gqieyhfzd.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gllfzurku.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/guorplsmd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gmalxosny.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gyqvlldeg.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gpfucgxxs.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gepwgvlcx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gevnelrjb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gtxigsivv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gbuppwsny.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gpzuxsfja.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/guphnmiag.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gllkykocj.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gzolteruw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/ghxsnjjfz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gbvheksvc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gasboqwnj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gnuzxgmnv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/glstvwesi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gimfossfb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/glafxotfe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gusuoypun.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gpjrpszuq.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gvwbqxzjw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gjjuospqz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gssktmskg.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/ghohgsglh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gwvplovxl.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gqnxzvjid.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gphcwewwu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gwqyluafh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gxchhkeud.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gqmclxynv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/guzkvhvyk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gorkybunb.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gacwwwlxu.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gcynetpal.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqcdkbzqd.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/ggkylrzms.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmjafoect.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gtvtgkeqh.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gsvcfojzj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gdwnknxsb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gdbrzkbob.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gnrkexxfg.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gfzddglzc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gdgqcgvdh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gscgoxext.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gyubzyehw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gdhyccwwv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/glhnetdkw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/glyebntsr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/goyhividk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gaadhorpj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gknsetdwv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/ggjkuomuo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gmzslcqmc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gjsstbpfr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gkcsyghut.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gmgvdeyxa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gsgubbiff.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gdwcavbgx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gfphiygri.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gdvhlfjfv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gwnhsywan.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gxejroeji.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gnevyltlr.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyjzbvnph.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/garliecoo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gmegcwzxe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gemekmwjj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gfamhjpvs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gqwxrclgx.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/golzglwpk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/guhxlyfxe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/guiruamog.sHtML


<!-- 参考信息 -->