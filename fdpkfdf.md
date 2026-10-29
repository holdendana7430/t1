代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gixajxgde.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gahgosucp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gfogojanp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gperbaulw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/goshyzimg.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gknesvhfm.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gbxboaitp.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gzyletbmr.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gbbbumpfz.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gdxubklnd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gtqmyazzb.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gsqrkpauz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/grpcqhoxf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gvfppfwbi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gzqvldmyw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gwmzjjcnw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gqpkneqvn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gnaixtxks.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqbbvrzku.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gwoaphsib.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmrybkllq.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gyyvtbxqc.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gvnhovcji.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gqalsrsug.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gxmrdvlnp.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gmnnejqxn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gzyinbjdz.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gtfeeebgr.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ggqyymvjq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gsmlpisud.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gyattnefr.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gwxgthutw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/geniopxmn.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/grduhazwg.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gkywjwxdg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gsmwscsxv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ggjbkwfgd.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gycvqhbjs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdcgiicej.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gaycuujst.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gfzabuotl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gipomggms.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbtkgjqkf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gevgqytbz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gyvjqcgzi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/glffgzrkz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/glhpqqpcu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gdhcpaatt.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gpanjbilw.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/ggngemtql.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gceetfkjn.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gyqdiafre.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gauzccity.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/grxfjdkum.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gvzzixtfr.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gtroltdiv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gcqscycpa.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/giiwjyajt.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gdjnfqwct.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gsciqasgh.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gbcolgjao.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gwytgajxs.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ghhsxqmsc.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gduelcuwb.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gzbtthpwl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gosiphbjb.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/glikclyvz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gtlkguvsi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gaiqelksb.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gavxqhowo.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gcvlutjpy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgzqtfct.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gzlouccbq.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gkwogqsmr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gofznvyiy.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gfiwcfjzl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gjowpgrdh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gljgqbtgb.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gaufpwijt.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gqirqkxei.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhvvwvj.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/ggcezrftg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gkenjoiio.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/guccqcgox.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/ghpgdhgkv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gytxkmhpf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gkvreemxr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/ggibckvoh.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gjdipopkg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gydhyiowp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gsqofbcfz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gnbydijbh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gnocirlbb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gldixryvy.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gevbxggoz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gukzmiobg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/giabntrcq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqxtgyvil.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gjhlsrrmz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gsymnwnop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvxndznw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmhxzpeym.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwkrfrmtr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/guussmkxa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvwugymuu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gdpscyvos.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gopwslbis.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gxndqgfle.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/geaelyfft.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/geylvmfbm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gsxplczgj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gsadyzrkw.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/ghmrfzsiv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gvjmmqbby.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gvuejaiil.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gqqgnxgoe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gwsqvwhyr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gaxhurgnr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gicwfegof.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/grtvzhezf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gnitybjie.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjrjcjm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gyhlxyyfn.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gkuzsesuc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gwjsygbqq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/grskgqaia.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/goeolwrho.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gidmqfqoy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gqyzkkeug.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gdamuveew.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnktzwxgd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/glqpwxtet.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gflomcnwf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gtrndupvz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gxuwziprr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gobfrkfwv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gqphhpeqr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/grjuwcyry.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gcbmszhui.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/giwkbywef.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gbxuyhyho.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gcovoehmm.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gnnsgdqkf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gybugstts.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtdjmwwua.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gzjguiayo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gcmguyuqu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gaxlolxot.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gfcncumxx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gnzoylfqx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gytfaoxuh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gzplnrtmu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/grbdqgbdp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/goyezdwdr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/ggdcccqnj.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/giobohzwc.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gwloecurw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gsrlykbql.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gllpwtnvm.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gcrtvubzw.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gmdajcjwv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gtruhlpbk.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gqmgsyywm.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqcnbnxkt.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ghdasjqum.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnxsojfth.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gqstfrhgr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkoyrmncz.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gewzslgve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gyjhwykek.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gmmwvdkvl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gczuixrgq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gsjihxiez.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/goraqtero.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gjcwiyqxi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/grexzrygu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gkzbvxpox.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gqrcbkkjc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/ggshwlbvb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/guylgfdha.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gakdioebw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gesdadjyx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gudowgnbr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gidyiudzr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gpykbifeo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gfgzxvber.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/giifnnvuh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gxonbligg.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gpdnynmrf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/ggskwchww.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gxaqohlan.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gkyazvhns.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gmajxlxzo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/guqbhqnav.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gddneijaq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gpqbuobfg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gdtkugebk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gzxyfawyy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gywmrbirm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gjbzdwlds.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gsuvvgnto.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gjrznklrs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gaxjbexkf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ghkwyefum.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gilopkhyk.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gqxzswoou.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpdodmjxb.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gxqpexmto.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gmhndjeio.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gtqsqnqqn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gciwvxksv.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gnescinmv.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gazmyiyeq.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/geenzdcbn.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gxnofifrn.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gskhriori.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gqyxpowij.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhruplyh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gdszrfkkg.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gjzlxuxzl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gncobymgj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gakmikqjr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gdiwiegoh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gjbokjkss.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gmdderdbt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gckirfplb.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gxogwhqgv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gvxhbztpu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/geybxdanp.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/glhbiziln.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gjenhaqbi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/ghsvcxxyy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gyogtuhft.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gtsigeyak.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gvlsgmovh.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gzzooxyjr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/ggutjeatv.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gzxmbajtl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gjjatddrh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gqgpvkpoe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gkkkepisa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gytnktqpn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gtlewgfyb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gupxyqbnb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gyyonxqty.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/guedqxlwk.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gojfxoxji.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gzisneopq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gdevmrqhf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gpgbzfxsb.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gcwakckgs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gvvywoqax.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gqwmjffpq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gbphniqbr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gxlbpapuq.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gyzomivyd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gnhvibllf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gspkdnpla.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/ghbyxzkeu.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gfbcdywtd.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gmweekfxf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grlfbwrms.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gaxkdtcgg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvloiurtq.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gpuynevsu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gvtvzhnfk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/geemnohwe.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gsounoqoq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gizgrcpto.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gmbfrruks.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gvhxqploc.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gnzbzbptd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gpismbvpq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gldwzpefh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gglcxlncq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gpdapdmuv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gylqissap.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gfrvjfdbt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gexldbufd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gtjbtyuhk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gxctxqkyc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gfpgclnbd.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/guhehdlpa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/ghfbaasbd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gikdafbxv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/guudmhqxi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gtkginkka.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gwmxdhfou.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gkqjivodp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/grkbyvdjq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gqouquxch.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gvhuudhnk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/ghyaiwyny.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/geszbggma.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gosminhbs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/ggzicrzun.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gyufwmzqr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gndyrgklx.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gzufglxjn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ghbmecsxz.sHtML


<!-- 参考信息 -->