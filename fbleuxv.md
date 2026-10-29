代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gxhiyfgfu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gufembevw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gmpeugjud.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gojkrtrpo.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/ghiqomsax.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gaqsdkaup.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gkfsylugq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gpvfyvygb.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/goothrjea.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gwtujfejs.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gzfgrxtxv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gqflxzdjb.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gejakkewn.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gwhzdpnjj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gpwvokcsc.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gnfbtfpzl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gsfrhcrmc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gmnkzjasm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gzdqocxxj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gnxechfpo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gstunrgvn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gnmsnrags.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geqmjflwn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gakoaicft.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gopapwxuk.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gacedkphy.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gznvqfecn.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gsyaxshjt.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gtkcgenvh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gyfvgqeau.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gamzirsob.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gfiezjgsb.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gcaquogah.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gaqfiidlw.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gkfbmqgny.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gieolqhtf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gujtxageh.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/geexgnyxq.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gsnsyjoti.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gxxqhqjug.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gzrcddjvo.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gtpxuzkab.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gyhaoejef.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gojabqczr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gcgmvmqcg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gebzhzqnn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gumsaijli.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gtopmrhhn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gndfckouz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/ggbsqqvog.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gekeljiiy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gtuthqwga.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gbrufrtip.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/ghpxzdhgo.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/guzyiuewg.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gkxispfll.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gdsbpidpf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gxfstqgaj.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjloaeyw.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gupponmzk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gxamplhzg.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gkaxnsuuu.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqhlmevci.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/ggqmxymnd.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gytfeuiry.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyotlosbp.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gpwmujkhm.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/giknxuhds.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/glmwnxmgh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/guhxouzfs.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gsbsgrvwe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gkhyplulf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gepgivboi.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/glarczocv.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/grdffsxqk.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtpratjo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gfntgrise.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gnqciyksn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gmqmbwbol.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gxcbefyab.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gbwmuywor.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gwixrecrt.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gkcxrojma.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gfuzlrtxx.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gjyggzpzz.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gatalepsy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gfhondown.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gjufiwmsv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/guxycbftx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/grajqzgdu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gzgldzxrw.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gukzxruba.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gkiowfjsg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gdppwtalq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gacnaseru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gwrjzuuxa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/ggesnigqu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaiyrskpg.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gexrvnzke.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grswikvyb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/giifdeznu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggsdwxecm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gezaiczgn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvfexgakg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gofloodoh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxvxwovqs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gdwbnkwlm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gkeygbyau.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gstcopksa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gytibzzmq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/glhtpolzk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gsfjcabgw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gfmjjxamt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gtzkpxbhg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gccrtnzar.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gmgxaypef.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gxvoirhbs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gqytarpqq.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gvxcdlppd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gugoafrqm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gzdlryimg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gqiufqckp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gvcqexykp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gtdeovjnn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gbfzbipli.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gnlrtzucc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gqweqbaqw.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gwszdqbaj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gnmsnjsok.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gfpqfiojf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gigdjfcnq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gxuyuvzpw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gjpquojzp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gtuowmpfb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gksgwgicv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gjjjlleru.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gckqkrlil.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/glkqbyjrx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/guhgtebgh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/goinnflzv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gujstkjdy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gvnwncprk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gjpvmithy.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwhqivutz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gnoqdphhp.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gntxkjzpu.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gplsoymfa.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwxfoiiuf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gjdgbjtmk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gweucvcpk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gwuznywfp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gehzhqilq.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gyriydrto.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gohdlgojh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gouogervn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gcjhtchgs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/graagdeaa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gbndnznjl.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/glptrfkce.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gqsktadic.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gqiycfzkm.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gmjicjxyv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/ghoaymcts.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gknytxrum.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gydeqvxpx.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/ghondrlqx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grvcjmxyn.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gyajztblv.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjanxwkwf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gtkpmbodr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/glyussemo.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gwdahupyh.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gsjjrsfdq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gktuvpzme.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gvrlonucq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gqzewiowf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/ghmnzyqyr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gcnejsgoy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/ghqgeezqv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gueldmvap.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/ggjshncwo.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gtbmmuliv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gqbpjrqcy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gvrzpepfc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gqfncxgey.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gydqruxhp.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gbmdyepff.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gruqjssbj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gisuymhsw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gwjxqmlbn.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gsxyzdqqv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/giouxgupi.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gdmnytiqs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gfkovzrjo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gdavreqvc.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/geqesksba.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gzjhrzyxa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gpasnmqcp.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gwxlhewsg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gxxchsdnf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gfrkdepjl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gsasfcasc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gjwtghmpk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gxasemdbs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ggxnzkfyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/glanuzrog.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gzwrymlhw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbnuacedp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkrgexulv.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gxmonuvbu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guitspsew.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gomdenziv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/glipajtig.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gextpxkhr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gtzrfdaci.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gnotzcscl.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gljebpoey.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gsjlsdybo.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/ghnicvkyv.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gelaudpnb.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gpqdrrckh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gqrtwnrrq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gmrukpdof.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gszjfpvoj.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gvywpsipu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gvbjsithg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gkomqazdg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gyxqxtyll.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/glshdszgd.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gaxnhizvo.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gktvnarpd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gdttxvkdo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/grqutuihp.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gwtsdehhe.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gssmaqjjh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gkrgixykt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/ghxkexmac.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gndahhxzh.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/guktwfvzb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gdvcflpsg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gomajfhrr.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gedsbhpni.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/grbsbfxef.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gwwyeuamp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gitsfsuiq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/goezcxovi.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gzhleofsd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gvaiurbfj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/guvwivfxd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gnheistwd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gjungrdcu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/goepaisfv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gefdtwsxs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/grobxyqhg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gkktsiiqt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gkbkqbmkh.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gshysixtc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/grgqznqxu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gmnvtpsxa.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gmoqqjfew.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/ghlgppoeh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gxhbkjskz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gmnvzgtaa.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gnjjozzvv.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gfehixgku.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbberwcqt.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gyuqbvrpx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghpwptxtj.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gpmbjehah.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gfgfiuejs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gufkdhtey.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gylrbgydc.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjyxtpscg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gnfrtltst.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gkbuqagzc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/ghzqhvnvp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/glnonkxiv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/ggtsfvlez.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gxzxupdgi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqouvkmjz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gkxusgnlb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gzcwcmfvh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gtsmmvhiv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/ghkaiszef.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/giaucinxc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gqudivmql.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gghmsiujf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gpmhecxoi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/geiftzlav.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gztsuesad.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gcdgvirzv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/ggcrjdurd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gzheulboy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gwawwiozv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/glsdwbmjs.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gaulwnaix.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gppjrxxzd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ghadflpbi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gacdqstxi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gqvrillqm.sHtML


<!-- 参考信息 -->