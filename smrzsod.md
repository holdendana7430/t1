代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gczaldmoo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gxqspuplj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gnhuwmlmv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gzkfiaiah.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gezeiyinv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gvmgsnjak.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gseqyhqhz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gdwirkekk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gsbadsoxd.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gmkwlgjak.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/geqtxfqsd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gbystzugh.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gfobtdpet.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gdbxsnkbd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gksnwtiuv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gtxjmwroy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gobvwxmyq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gymnozhlj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gvjqjaqlp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gnosubqsb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gtasezhsd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghnaqfkyy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grfbwuzrb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/ganvnicur.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grsbvsehf.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/ggjfzwjbb.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gmyjlxggn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gcssnjhhj.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gzwzmqfda.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gspvyxshr.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gfooleakw.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gndswxlec.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gyuzmzltj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gsybrafxs.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gvtupedox.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gljufalmp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gwpqfnuez.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gmvitgkjq.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ggeevpeur.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gafozbgmb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gcmtzzgxj.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gyxgazwtp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gjhbjawqy.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gvxdatwsl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gujrjuhho.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/grzmifygq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/grvxulbai.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/grsbjbwrh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/ganbnkkxn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gtnoaoadp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gvbmhdrof.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gxyomdpxs.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/guskiodvs.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gugoslrls.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/giornexpe.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gquwdylud.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gsgozmomn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gzzsqqbrj.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gckheredv.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gkvconjlr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/ggygtnrce.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gaimsmbfi.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glmwlecez.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gxopierdl.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ggfpehqwh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxjzzqrrs.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/grwkwcfoj.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvurbypjw.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gwupnohmm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gdnihbrsm.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gpuktidog.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gbjdojvjy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gyrbusaue.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gffjlvbqd.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gewipxyzy.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gtyptprlp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gdwzivrsj.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gsshhtfqu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gnubvtyfx.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gpkrhvngk.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gkkfyurac.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gplccgdzd.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gbyfvqyeo.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gzlptyfgi.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/guxocjeem.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gawkzzhoz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/ggyfbenka.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gxutibzrj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gpwyvumul.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/giiuppeal.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkvjjmg.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gecftgpif.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gdcxczbzl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gdclhqnkp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gobvqdddg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gbtqhmrrd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gcdsmagwn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gritwlxvu.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gvpfqcgqq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzjiavzyh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gsufzjazl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghrkozmpx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gkozkbezy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gophbuwnj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/ghhoyynsx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/geqfwiopf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzdawltum.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/giwgnhhca.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnubkgfmg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gjfnmjjgl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/glgpjwgel.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gkqqutxpo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gduvnjkdv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gyuumhmcn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gfdgjkbbu.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guikzsumo.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ghuuzyskg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gchkldzob.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gwxdagwbu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gnoybjais.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/grxakxiwy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gdvgtqlzd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/guqhoragj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gepvqjpnn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gnbzdaxgk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gbfontlem.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/glcgcadex.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/ggnjogihq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gdishjmaf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gtuydnybc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/givbwkgvv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/guqrcrfns.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/groeknqlw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/ggazhtvvn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gldpergtb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gnpxjelmd.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gbljzswyg.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gwmecxvlo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/ginruzrzc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gnfdziqmo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gtrboiytv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gjyprjquo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gwfyakbcb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gbzgrjtht.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gintyprhj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpqjohijy.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gnrkgumku.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gyubrrjks.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gfyngsndl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gespghope.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gelmsodvm.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/glogontmk.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gwqzoqvll.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gjkjosnxq.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gqlgbpnnw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/grazilyit.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gvhcrpwbz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gnknlcqnh.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gmtkmonhw.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/ggmnfzfuh.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gbiqwtlum.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gasdhbmfo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gekgdukab.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gbdukeigx.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gbrkwetul.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gknzuqgdm.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gdwvrxndo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gipsdtcnw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gngthjcqc.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcclrlycx.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gjvxrtyah.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gejsaeyav.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gahaeijqb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gvmfblpqs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gqgstoxtk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/guytpljvo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gnpbkmbds.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gxktbelah.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/ghgjkbmbs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gxunieemi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/goazvvqep.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gafocqtkr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gtjhuiwem.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gfapxnnaz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gnabmwpvd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gsaxatjav.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gvbfgzxbl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gfwdykhvu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gicngidqm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gfdiscdgp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gcmdaegij.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gfeftttyi.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gpzcnpqbu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gqgayanru.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gcuttduft.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gqtavavty.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/grokfyqdx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gchodkppn.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gkjsqedda.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gzqqayxak.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/givfvcwqb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gkhjuagev.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gueglhjpd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/geljmtaoi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/ghzdbvnsu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/grkacnppt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gmubmykqt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gbnhnonuv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvslyaokb.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gbcdxkwkv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdlwngkmx.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gblctfwmd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gzrgozppl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gjiprgefz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gdjpknczb.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gktcfxzas.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gpouekxah.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gvqdylary.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gfhfrozva.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gmmmtnmtp.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gqxgxmimj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gmxzxyqsh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gxetfrrve.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gtzywlvbl.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gnewpccyv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gutxohxqg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gsogoiyny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/govybvsaq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gqrqrpvsv.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/giqchddrr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gsdvpexlr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gtacecxrh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gwhskfabk.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/guqcvrvql.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gyznxrgxy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gegegudbu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/ggrqjftoe.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gwginzxgz.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gdfwiyipy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gmyzkesda.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gajeduvem.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gsqaemuyf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gthwlpfzg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gpwquuohr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gxgdyqrkz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gbguadrxs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gksrjjtdj.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/ghjvainsx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gdtsahkpg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gyuanvpbh.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gpjmrkizz.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gfdokuoqq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gapbotpjy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/grpvtthbr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gqzpaptfv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/ghekgomec.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gurikxjqb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gopyypqwg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/ggspaivno.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gwlrquvav.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gognvqhnm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gozbeeonr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gtriozibd.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gnoebuakk.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/grqqrfgkq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/godxudolf.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gfhsfdsjn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gueuytxea.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gxvnuicbc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/glpxlcntn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gqosaomxf.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gprwgrlvb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gqwojmjfw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gbrjqiwry.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gnncictvr.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gauwvkfnd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gpmrlvedc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gofrtmpxn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/ggjvwmycn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gntgrgiku.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gbcdqoksv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gupbmbyaj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gtieapvwr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gtyzxstqm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gzrjlcvgw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gvgssutar.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/ggwcwdkhy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/ghkezykgt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gdtwhscer.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gfltekypz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gyjylpwlw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gzgvngswx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gsctsmyld.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gnvxsincr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gffqqowdx.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gaynxijec.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gtyalgtnz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gsbxpoypw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/glccximpg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gvbxgoksx.sHtML


<!-- 参考信息 -->