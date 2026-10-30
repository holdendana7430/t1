代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gmyokyvvg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/grnmynypd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gfgtkfaxc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gpbyuwehh.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gpdnwnolf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/giechrhmh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/glwsyqpwc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gxjgeryaq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gpghkfgck.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gzltxuzpy.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gkzvusqxe.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gysaxxrjr.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gqojizzjg.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gewzeyoqj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gnwlpjrbl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gtbkpbnhe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gtcntvuya.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gyyilxpnq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gqsuimtlp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/ggdmfnsum.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/giudzdqsp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gaitihczg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghrqnnntc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gcswbrewf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnathbufs.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gphifperb.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gsdztjzqq.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gxlvacwyo.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gwlycaqns.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gdpcapftf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gkfacrpqa.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gkssdqswj.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gstqybmhp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/galhcqtty.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzbcjdxpr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gajxxobix.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gssnbmlox.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gtkhdxmww.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gyigsyjzf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gslyilyqw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gijjzodul.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gafjihfcp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gpacbywgw.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/guzgmcxnx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gxtcdalhk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gdleroijs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gegszkqvc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gfbbemsza.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gjsxivekr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gmwncnfju.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gdzrylsdg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gimpoxrlk.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gwajetdya.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/goulypozu.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gbbkmboqo.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/ghsutbddd.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gefjiypqe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gkxkuqjgi.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gyffsqlgc.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gbaxvscwb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/goydjprma.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gnypdfdnt.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gijvdcwiz.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gelzownbt.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/glzbalfzu.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/guzourvht.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ghqhngvwl.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gqwwiiixk.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gtimutddt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gfessgvon.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gbmuktiae.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gsqwrtfny.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gwrmcdtho.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gvibfmjaq.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghsyfyokr.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gfawlxqpy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gagojhrcn.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gktakpvzh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/guiojaqyq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/givkapdkl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/ggdwhwkbm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gkdwzewyj.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gooylpnti.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gdyqebcgk.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gfapuembm.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gqruengxt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gtmfgdvaq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgrqplsg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gijtplrko.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gmzkxawah.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gkxzlvnqs.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gdsottels.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gxpmepjsg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gbwivjsas.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/ghetywgab.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gmywhhaxf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gxrwlrkhi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdkphnjnc.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gpegephas.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpjwlds.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gqgmimbbd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnohfditg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gnisjlhbo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gghqsvocf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gpntfanao.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnebedxgf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gffazumjo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gwonmbjfq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqhvkbjiu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gzhgysali.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gyunrbeuk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gknnaetfa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gnfwqsrxn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gmaxemasm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gnotrggzi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gdgljttuf.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gxpupcfnc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gumnloodg.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gvxoeobvn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gxrkelkkj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gmmbjqtkn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gohemepay.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gzcjnplbu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/grlhqvvro.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gyhbfnfer.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gopwolcee.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/ggjjumbca.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gyzpukyqy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gtuuljrxz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/golbfyaio.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gylubjthq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ghmnqmgdg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gxhlnqrfc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gxgvljyxv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gyegpjzqf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gddlhitvj.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gagwxbeml.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gwzwcvske.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtexzrxzy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/ghqbkwurd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/grjlpjogc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gkggyjmhw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gmrujpddk.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gbfaswsjy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/goafjepsg.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gcqtaynpm.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gxbktaoxi.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/ghseujmnk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gntidwcbp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/goclbwzoj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gubzxnbrr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/growdoaij.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gufatbepx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/glgkevfqu.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gorneumhw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gqskamufa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gjaoiymro.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gazoqdtog.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gnifgthwj.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gfuscdmvc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gyshzefcm.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gaytozqxh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gejbmplsz.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gpfyvzkle.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/ghksujeni.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gvbjqmwml.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gggjifugz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/giuxqjfnh.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxpfugioz.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjwdrpisg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/glyaxzxkc.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkvkshhzr.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gmnijghvo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gkedqbbch.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/grvvqkiuq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghslpefrt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gbkvhcpiz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gmqkckmia.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gwkkhfeka.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gxypegley.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ghaphxrmb.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gvqvkliqj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gxmibbwlg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gjrxmnmyo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gewiprybr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gsbegpmmr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gncifonne.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gbhxspqyn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gdxhfjmom.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gwkffqoog.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/grrjdkwyl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gnokyxkji.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gmkstxasy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gospugvtn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gtnekwdza.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/giqgmteil.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gxccbmwjg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gfusexvqc.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gpbejbfjq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gpkpliwkd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gqnnngwvm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gyilerbvp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/grbsyvpov.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/glcqwuqwz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gjxkaucmu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gixknclxk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/guntovtpi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/guidqchsa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guvuuhcor.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gjvfsshmi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcjnmixab.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gdedkkruo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/glymrqujo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gasspwsme.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/ggmgdjcmz.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvugxxdhz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gmxawgrzd.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gsyxkxucn.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvqgarck.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gtapgrhee.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/grjkziokk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gwztjvnmr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/ggkokrjmn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gririgqnw.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gdbfnvynv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gooyccked.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gggeoyzqt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gzwgwboyw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/guiphoeaf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gurrcmjgt.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gtxfpvkvf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gybumvfvs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gvpfvtfig.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gbgaftcov.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gqfngtxzv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gegdxbdxf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gxqasmrug.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gqgwqiheg.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gebeflkmk.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gwsnroqhh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gkcvceyzx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gzcdduuyn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gtmbwzamc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gloxjbvoj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gdzrvtrgr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gjhoxegxw.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gjvjgylsr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gdfdxyfsw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gchxwuzhs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/ghboanfae.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gjywldxci.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gkhtmndnb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gkzonytjs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gypjyonrb.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmcjdpc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gsbbihewx.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gwnlofsje.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gpizkkvdj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gzrobqfio.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gmbvdtmig.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gmmqqydne.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gtdpikbxh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gngyrlogc.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gorvsrqfe.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gsgcmevkw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcoxnonrn.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/ghgxfwhol.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyusywckh.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/ggqtfsvzu.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gxwawbxsl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gdltdfwbl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gqmrxoein.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkracjsjv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gilpkdwwn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gcjnhubef.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gjqqtunqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gylmstcwi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gchzhrqdo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gmqbsqwpf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gchjgkqpt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gzihppyty.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gqzqylwey.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gbthagmon.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/glhgdtzjl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gudwrcnsx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gtqrgbxow.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gdgvlmesx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gevopgjvs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gerhaloyf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/ghcujnedy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gpzymtvvh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gvsskmfre.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gamtebrkw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gbsasnpdx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gnulieyzy.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gwrctdaom.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/ggirgrivk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gylbiobxv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghmbtthil.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/glhengffy.sHtML


<!-- 参考信息 -->