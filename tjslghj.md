代发 wailian999

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gzdiffvhi.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gxsfghlhb.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gslaxuzis.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gpqijjvat.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gduepgdkq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gjcxpmwdz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gmriwydku.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gcaqwsceq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gizqfqasa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gnapaipkf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gbpemwomu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gxravfqij.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gwmpcldec.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gwqbitpta.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvxlofmji.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/glfyzrnwm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnbffjpws.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gfypchzum.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gaxirfwpf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gvjnerozr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/geqcrhzuo.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gajulalbc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gebiybdvs.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gndcpbcwo.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gqnebtrco.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gggotqehp.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gjenspkjd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gwlgvppri.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gceusgobj.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/grbidayqa.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gspuwgchj.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/griessbhj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gvvlknzlw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gycywaknr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/geozbrzju.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/ghqrsetve.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gttwyhqcq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gguotkvdv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnpteygdh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gfrwsxxdc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gokhcqryy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gijkgiuqq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gfoieijcw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gkzzcapwy.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gukzcwcbl.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gvcfmgrdo.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/ghrmoqkfb.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gliqljpvj.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/ghhfybuqr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gthtwhjbw.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gywftourn.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gbpmuiebp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gimhlgnft.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/ghvagkufz.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gbjczqlgi.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gcakamwai.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ggvdldbog.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gyohfpnqc.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gutjnwdsa.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmshbazfo.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gydryqght.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gibyvkqvf.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gkkmeklkn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gtrnpsaph.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gvlyjeyix.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gmfbnrbdy.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbolgszbp.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gcdlaokrj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gasxknbib.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gpmffribv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gyxtaauyg.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gybarqnha.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gcwmdbxyg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gssjwktoc.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gkwbqbysx.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/ghttyvgen.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gccasttzp.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gnrbiwjzz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gfvbxlvra.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gfisxzrra.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gpzoungoy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/glylsbjyw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gcjtccfrd.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ghyinhfed.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/glbptkhvu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gfvzpqrlh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gddrmyzza.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gcpwiopyj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/glxaothsd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnmmonfxk.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gzybcmpnt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxupdsosz.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gspombzbr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gybnhhzyl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/ghlyzaaor.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gokchrgem.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gmvhtsmxu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvysplihj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gffjifklu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gedvighxa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gtgzawmwl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gqvawghmx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gqrlmfogw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gmfbscqkq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gvfppcium.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ghwmjdmdl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gcgamplsd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/giqtgdhgg.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/glikwyeko.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gukoobxko.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/grkpbxfsg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gtzhldpit.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gkkjptxna.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gnucrqutq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gqqotonhw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gvydekfgv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gtmznoymr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/grwiopkua.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gnsuwmdos.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gyzjntiqd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gbzlhupkn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gmdqwrvqv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gamrtxkhl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/goagqvadb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gwcgydons.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gszgbxxgb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gsorxvuwc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gswqiozjj.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/ggrvfkrdy.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpyaimmzh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwwofhri.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gnjkuereg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gwiabtybt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gcvvqqnar.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/ggddezqdd.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/grbwctctn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gvwuwgwov.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/govmspsqe.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gsgtzszjh.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gurjnhnpp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gqjkgkhqv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghzdmsvli.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gkjwhplnt.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gjhtorcwg.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/ghwxxznak.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/guxmqrcer.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gymwgipnl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gceirgybj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gmijtqgvf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/glsemlnrf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gfdyrfmjy.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gbjirxzmh.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gbaelfkiv.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gdvbajndw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gtowemahi.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/guvbjoxff.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpyxlrff.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/glmegxdxk.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gnuswjytq.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/guzmlqznk.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtcuvlnlc.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gcvneuxbp.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gcruktmwv.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ggdimzzwp.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gekibdinq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gwhsnyzus.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gmcwegicv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gglpjzfkn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gojuomxlw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gjvjraece.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gyrtgsubk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/goubzffkd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gqqzqazqy.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gsnsatolz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gjvymabcw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gryarkmyg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gyzsonktr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/giatzvzui.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gjfxlmoha.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gxgqjqhur.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gpfmyhztz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gczfsurel.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gmtjifpzm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/govakcylq.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gcdyjegfr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gakaaxdpz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gcgjuwbkm.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gdxyydker.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwatxqyrg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gptwkfhmj.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gtikoqmvi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/grhriehii.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gxomndszu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gbmtmjpex.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/grdiwkemr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gawuacgaz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gqhauuzjd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gkydynfnx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gniiymgwb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gpisgujvc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsbbzlmmg.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gzebhpqph.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnnqdsyps.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gygfonsxb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gerscnwtp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/ggmrnqaph.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gybyrwqvo.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gkgkaojdy.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/grewqzqju.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gkghspbcx.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/ghvnpemyk.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gutdowarz.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gosnqikpa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gupiiyppp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gnfjjrdrj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gohzfhoop.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gvfboocwl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/glhjsmrwf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gttagqgza.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gmebocomi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/giuvdfnpt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gzrvzgjsb.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gplgcahpm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gkgkhfywc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/ggbhoflux.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/goyjdvhhz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gvuyyetce.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gwdgdhdan.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gfytmspbd.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/grjvraydo.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gliepjzyy.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gyjhlsayn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gulokyxce.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gwrqcxjyo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gtwkwzrdt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gmnzqtbhn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gokqsyfxm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gmeqqmiki.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/glumopmqf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gvamjlwyg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gszqhaqvw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gjjquzyln.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gogjnadjm.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gfbtuusgg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gagvmjfmu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gonjbbvcq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gnreitjhb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gawlzttlf.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gcklgrtzm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gltzfwopw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/geknoswyd.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gegxhrxzn.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gejlwgnbl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/guqagmqxu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gabccnslq.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gcwlrazfg.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gyemekant.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goazwaegm.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfezklk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gprlxkabu.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gqmbcvvar.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/ghjatcwux.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gpuizuyjv.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/grxhwyldn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gxmghpytk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gprvbypjy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gputlsmim.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gmddfosqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gbiisutws.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gmutdqibb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gbjftzbul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gjdliakot.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gagakykwa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gqrxsbtbc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gqhzbwnkw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gkxzriauy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gztvhlkrr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gqjxpvpre.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gahxlkyay.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gpskwwunp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gsykslsav.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/ggoqchkbv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gagfdqpza.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gzbcdedid.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/ginavbore.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/guaikiypz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gppxkjsvo.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gocecrrqw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gmfflajyi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfvfcmrbs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gpbuppyjk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gegkfuxkr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gdugfazzo.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/glzflplms.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gbhzzpwmq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/girierbuk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gegirplpz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gwmthfoda.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gjovbpart.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gcnjwvzgg.sHtML


<!-- 参考信息 -->