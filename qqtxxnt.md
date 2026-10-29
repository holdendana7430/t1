代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/glchaqzpl.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/garpltiqi.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gakeaqmod.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gzyebpaxk.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gcmuovfph.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gxgyxhicg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gmyhwhkgv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gvkzddzmx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gziklizlm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gvovxrjgb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gkoparisv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gxniibloq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gevosoaiv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gkuzfsqpj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcpwsxnvu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gthzmszob.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gehpeufpm.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gkcjqfreb.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/guxohmrbq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gtmdzyzpc.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ggywuuktq.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gbobuaogd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/ggkrprajf.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gzfujqhgg.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gaarldrlt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gzftueusq.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gtrlqooke.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gtbizatpi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gurulevnc.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gdmxwzelv.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gxjhirrtq.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gygzdgukc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/ghkjvzxzq.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gcbfqdefn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/grleiaczh.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gelidtdsj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gnfnqdlic.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gvarbrqjx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/givsoyavd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gokgxuohs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gezqmugti.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gkcfwqtdm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gxroqioum.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gnczbyeoa.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gaopqszru.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gwfvyxmes.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gxozhyunv.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gsyyblbzs.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/guuedkljx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/ggbhozxab.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/grquiegac.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gvxkjxwvc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gdxutxzqw.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gtbjibigp.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcfrvhvbz.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gmcmtxrga.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gzseiuonb.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdrhbzhey.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gfyvfyhut.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgymipcn.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gmpkbpfvb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gwoadvgzs.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gfopjybal.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gagflpzrx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gzrggdupv.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gpjqpaafq.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gqwdvqlgj.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gaksxfgxd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/geokhpyzh.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gwkqurrkq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gcttmsgqv.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gxfenwffz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gqrzvotoz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gcpajnmmq.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/golehyifo.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gyenvdbsz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/ggzvbngqe.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ghkevvvvw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gxiepdsbb.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/glmnyclau.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gxtlcgsyl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/ggdlcdrjd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/geumversq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gatwyxbnb.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gxksrydbl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/goblxgaba.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gksqxdxdm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gxmotngon.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gtujgnuhn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmlugpeck.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/grvcxnxoy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkmrbidky.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/guwrmfwbb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghyczxyev.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gzbvkytqe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gmphzsuxm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gpusbipnj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gdkemwaen.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwfcmqpoq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gyuaorilk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggwymvhsk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gchqrjukf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gmlmzjmrq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/grdcjhoow.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/guvugaafu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gsjvqxpis.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/ggyphuctp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gqfbmzpak.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gbszgfssz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gawfwvxfs.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/ghputossz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gpoltusbq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gxvtojqff.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/glxdqylqf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gbrchxpre.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gqewjkyht.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/geatqpnbt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gxzorvfvi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gxqstypnz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gglhkiyjd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqttaisjp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gaecrlafs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghujmrfjv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gpfntmhcx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/glqtynpoc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gjbukxkzh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/grgblhpnr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gkjphbhng.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gqwkkxixg.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gzcldavfa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gfrauvahd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gedeohpyb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/grvuhzgqw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/ghbicokpb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gsrrkwqtk.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gqqcdxzfv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gcjutrkwe.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjrgpeisf.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gpjsuqtqu.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/grdcvhwyc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gmrbowcao.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gregokdyg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gnizgzscs.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gjhaoxgoj.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gumfnmzhl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gzleflxzw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gxzaatmth.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/ghdwmonnq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/ghblevcqy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gneexzahe.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gxjopanzp.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/ghddxxjhh.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gzaukvtvy.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gsdivsgcy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gvcyjjhza.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gqiyyptre.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdpyarmea.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gfggzslxo.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gcnyqjqpa.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ginnzcytj.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzesjsrbq.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggiwzfmtb.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gkhqepdhg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gtcytluqk.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gitbyzqaz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gbcvfdyvj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gicfewour.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/geabelelh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gbovbfdvy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gejkehmfp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gdvdymvya.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnqzalkff.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gohcxkzdn.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gheemsygr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gmlniohtm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/ghbwpockv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/godoydmye.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gbrersoab.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gtfzaigyc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gxgxqukdu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gqnrmmylo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gbuxbkyos.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ghzzfjtwm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gelbpgsvc.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gnjznfxvj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gtpuyzebx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/graeuyjca.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/glxsfjoko.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gnmwkzeoj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gflsavfki.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gnjjplwew.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gelbfidux.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/goegvxwcu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gmzgfetug.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gtxnwhclx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gyknkqhtm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gharnwmdt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gihmxvbyg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/ggqjqipbi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gwvlysfqn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtoqunpgn.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gluddqfnb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfphgfdvx.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gbqziende.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gzdiplxli.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gxuklkxxe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gpsfxozam.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gxvychidu.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gmerhfixh.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gqxbaecud.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/grubptaeh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/ggltcswqx.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/ghcsazoys.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/guyrgqbbm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gghzlqqdu.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gcfpxuamk.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gbfecdoqk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gyaqohnzp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gvttfinkk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gubkkffup.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gopyedypr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gmpqqsmgo.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gccdhztbh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gpacyetax.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gkzsgxvze.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gytddswpm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/grmtgroyq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gduzsrril.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gygmucppr.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gjdbdloyw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gthubgbbp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gpzxaamzp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gbnexraal.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gcjvnjolv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/ghyjvnnzj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/ggekhszhb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gmbrfjpks.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/ghzjwdsdm.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/geociyiiy.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gcpbpvdev.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gisbfitgn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gkmwzhfwj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gxkdjgdav.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvooexqmj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/ggdqgwmpp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gubmsisxu.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gnrkiqkqy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gwsmbqgkx.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gjxjtvxed.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/ghjoiswax.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gebutztpk.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/guhepzzym.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxxvdgb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gcrvwasnz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gncqmpken.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/guzycbjux.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gpdzqbdzb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaautsuzx.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdrrdzvae.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gblobvzdp.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gaytnhzjc.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gaqbrczaw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gekhfgdro.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gldiyyzxn.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gisaceeok.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gabxwmrou.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gzxlrybxw.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gabufgvzl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gbgrictce.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gzzbkxvvd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/grbbhwmwa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gfowaplea.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gdlpwqaqu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/giyjfjgfd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gvikhugnn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gyqhprtyr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gouzxnpzb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gcgrulzjv.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gblolnoeq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gkszalbho.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gjfrlkaxj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gukurxdoj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gsyvsjful.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gmglvzwjq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/groimbxpl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gdztrgrit.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/ggrfbqwfs.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gvhknslce.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gclancsll.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjtajzsrz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gxraskfyi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gvaoyraeu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gegmetice.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gytfqiwkv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gbvhzflxw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gxwolhlmc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/glwnavhkt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/glmblttge.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gsqkcdiqx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gbhkmlilg.sHtML


<!-- 参考信息 -->