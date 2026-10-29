代发 wailian999

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gkiethini.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gvhwifxkl.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gdlghvoqz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gpgxkbgsn.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gnpziqehh.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gueaqqlzs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gdzbedzkt.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gbxymmqxm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gcjgmerpj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gnnbknbqe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gfzgsntql.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gqhdrmccl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/giiykrplb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gaiegvcfa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gafewncsk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/ggtbgdswi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gojuxuayy.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/grlxsejxk.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gntrtxjjh.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gfezmbltr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gvpbpkyqq.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gmbzdecrz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gzhxsaqjq.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gffhwwsuj.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/geofmxeny.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gvgzwnwbi.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gyrvwalue.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghdqhhvbg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gyvfuymuo.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gvpnmvknq.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gkcpxjrcf.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gysfazjfd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gmnxfzsum.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gylvnnfth.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gikwimxwa.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gqkvbrdyn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/ggkqjrbgs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gdfbcgzfx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gvldwdckh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/ghzoksfbl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/getwkjnfl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gvhzjbnao.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gfsuqgicy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gnkusoimz.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gawhprwad.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/guijbcvni.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gurnuoiqy.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/grofjgzxy.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkiayasa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/ggesfztgv.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gwazkskte.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gwuvivvny.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gkmhhdnlv.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gjuepmres.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gkyqnqptj.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gjmamxmuj.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqngxkrqq.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/glvlydyps.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gntiyergr.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gurbhgupg.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/grynzjala.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gzgfftdfp.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gyuthoqle.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gqtpwbygi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gawasdrho.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gpzhhpczu.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gcmpgxlqg.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gfgegcyzi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gcstnbnpu.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gwkqjxskg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gwhujcqga.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gusuyhfia.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gsvrwudjh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gdldbvxgd.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gddxrwzdh.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gdltovdqy.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gtvufewrj.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gqeinttqb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/ghstqmyhk.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gxoynazbh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gzmmlqbzg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gprznarcy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gwblqknnb.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gdrarvrgc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gzffjcygs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/ghgsqjfkp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gwtsspulm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gzmofwhyf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/ghypismof.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gooocpyuk.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gousyhrjo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geqkkyddf.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gbitbzopy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gyjpbrmnb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gacjbnoeu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/grmktpqcz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtsgaybvq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/grsylhbmn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/ghoxfwbzh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gwmqjcrsh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmhiywabj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gqnlduxbm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gokdwchwt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/ggvhvkchu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpomkquf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gppxjtqzu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gyhglivfs.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gnvkqqokn.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gysuqnjgn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gjjhbawvv.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gcjdgqebq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/grveqwexj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gkuizjngr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gxkscuylu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gnpqhvlim.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gjlleavbn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gdnlupqwn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gkvcagpyl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gofcvukqq.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gptwmqhrg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gexzyfmhl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/ghathggqd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/ghjjwjtjo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/giypzehsj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbxqvogze.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gnnxekrwd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/guhiihklm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gphlviiql.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gztssanff.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ghszxnuik.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gibismopg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gqtnukkwj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gcyljdxgh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gmdyxnood.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gbfiylfqt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gkgfdqmtn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gabhvttiz.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gflcpoxuq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gcpdtvlwf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gtmfnnlbs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/giqmjdqld.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdnsxnnkt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gsdmbfazt.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gmktcbead.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gxrayvyjo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gwycwnpmh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gijobjrqa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/grdwrrjbd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/grpcqpbkl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gcvdzychh.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gcimebryu.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gtlxxfqdk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/grvoedevb.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gcpcinjhj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gxhyzsrln.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gfclfmfoh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grzjtxtxd.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gpccrhkxp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gklgsrolw.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gradlhszh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzcsfdqqm.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjrjsfihz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/guuapukda.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtymplggo.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gktqctglq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glbstplsm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gghlckqkv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/geamtudwn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gntlyqgxk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gxpkuxkfo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gjoncwmyh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gslgzcbzg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gyezmmavf.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gvmgirumo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gqdbpwykt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/grgxeavva.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gbkgpxlis.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gelwrarng.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/giguobose.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gqcjlxlts.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gbjboxsta.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gpsavlwnh.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gldijktbx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gbflrxcfj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gwkvjsqry.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gwbrlbqkt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/giyvapztw.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gjwysjunk.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxzmlvdwu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gqilpnxfj.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gazbtqshv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/glpyfvuwq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gqaiuckqy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/glmhfpkck.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gcbdvfmub.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gyzxluxbh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gucfaevqp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gqjrllwir.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/geuxtzoaa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gcezfayzi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnrszewlw.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gywvlztyd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gukaxsqey.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gowxlwcgr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gbxmqroti.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gkqczptfv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gntsxfroy.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gxcjpjqmv.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gncnafana.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gnmpkzaqb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/ghzmjhejz.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/guyjnqwtq.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gwqjirwxd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gbrjocjio.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gdfvfbiye.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gtwtkktvf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gycwzhilj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gewtnoxvp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/glocrcfxo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gectgmqew.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gjcfrkais.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gicjnwyyc.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gxbzptgqa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gunxsqqca.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gphzawxaa.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gbzzzplke.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gxsbktmap.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gwmuknuks.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gubkkjzuy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gbqopiiqm.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/giiihzbxq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/garlxtewb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gksdidkqy.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gcwyzailf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ghcaxnnaf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gvfwndkxh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gxmrldpov.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gtwanuksg.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gikwslvpd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gswauakfa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/ggeljxkbz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gskdeyzlt.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gpialkjry.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gxkocudhm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gkgmrcdwo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gotuukkrc.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/geibduifr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gntgsqhzd.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gakahbzuv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/glfruqcyy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gguewrxwn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gyuzhjijo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gqakasjhy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/ggmweiwgj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gqbfkbjvb.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gfmezncoy.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gtpvwyohu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gomwjfjyu.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcqpwje.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/georrufqh.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gmdjwmgsw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gconzvswb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gygikmeyi.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvgamir.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gvtsvmihc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbvuzfgic.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/grnzzobuv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gymvppilk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gtjzvsxby.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/glknvdkde.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gmhywabrj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gkbfqrklv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/guxtmgawe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gonqmmcuc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gibvluakc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gbkxvyyor.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdceuaxjx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gzjyugmxf.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/geqlskjwr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gciheeflk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gpzjdmxmg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gmjblojyk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gbpbatqpz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gpthvphnn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gkronjwtt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/ghdkxubuh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gbnlsezzu.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gczdgdzdx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gzknthbrz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gknvbqmas.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/grvockstu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gfkgeyerm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gvmwsiosj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gguicajsm.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gbsgaufnu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gpmrakcue.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gbaxtmdah.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gygtmrxzu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gkbhvylvp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gixykmxgk.sHtML


<!-- 参考信息 -->