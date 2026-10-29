代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gposzyctq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gbcvnhsgr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gdsxolkoz.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gxgmmlxrg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gqbykoqzl.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gxjiswwib.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gvoocqweu.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/glkktfufb.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gbdeldxip.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gmsrxuetd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gywdmnmca.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gdcsfznko.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gjknrabfr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gnexkaavv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gcuormjks.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gsfmsodnu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/ginkvgwpm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/goftccacd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gudqqvjtp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gmmllpfba.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsvhduill.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gopvfloxq.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/geftfuzrx.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gplcqtaro.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gwsamcmil.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gmjtmcufq.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gzgsjsyxo.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gemvvlgvd.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gdqibokpu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/grnfsxpio.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gwochomch.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/grithchri.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxcjprz.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gqffzyavk.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gskmwraek.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gqhxkbbca.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/grqxhvgtb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/ghhwbucfd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/grinqivbc.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gtbxcyjry.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gbneqsgis.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gouicblqu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gjpdfnjcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gktsycshn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gvleblmqq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gauqxenqq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gykpefula.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gxjdgiowk.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/ghvscjich.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gsfsuifix.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/grhflxiol.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gzuvlfekd.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gtyodnenz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/goyxvabxf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gczecpjil.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gmzadnmzd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gwwyrkojq.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gjsrvlvnm.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gxcqoxwmo.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gvrffqeqd.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gsudruuux.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gogbsnbrf.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gafkapvaq.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtsayixbo.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gdsjbifrh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gtldvephl.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gbqlvgxyn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gwkjbczjr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gahcerhzo.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gugifxmqt.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ggwublogu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/goquxtxpu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gxbncdduu.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gswkhbuhs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gghuuxvca.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gxjgzkucl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gbbugisbb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gfjqfgmxa.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gopzssagw.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glghydrsx.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gnzbylzqa.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gwnotvhok.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gfihsqohf.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gqsjhzjxv.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gagkzcmhb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gnhmonrjf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gkothxuyy.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/giwksyqtq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gcnnueyzr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gvmazkiho.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gurgthehj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gsserxhzw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gphwjttws.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glbancnde.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ghfnauhfd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbtlmaazj.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gwuusfwuq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/guyoskyfr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gkecstsiy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gxobyxuhw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gtejmhbbk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gfcjdrzah.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggfcgwlab.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/grynzlcko.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gewnonaon.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gyrfcemzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gjvrdjgrp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gobynydgt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gvsqlwbxn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/girgbnkui.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwnbkcmu.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gwaiquzwq.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gkdrsejxv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gayngjkfz.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gqdovkyai.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/ghmlvirej.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gwlfooyyv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gdghlzafd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gcsksmsct.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gqqhbvpmm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gammgtism.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/ghmadxcmx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gejorpxsy.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gpynwiwgu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gstifaynf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gxmmmwlkb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gdedxekgm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gwrdsdkmw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gvfazuajh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gyvkxtfnh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/ghljrpubl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gnjltabdg.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gzntpwirq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gbkyjhzsg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/grotglkgx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gtcomjlik.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gbirpzhig.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gctivgmiu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/ggrxgwuhq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/garujwdjq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gycwwxhny.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gfjfqlgmg.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gyzsbxbny.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gwhlxyrlg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/giznpydxa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gabtttugu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/grelplpng.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gcbxxgnxr.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gnjhimsdh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gnaexqetm.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gaialorra.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gkgbrwrmq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gbxcrgkjw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/ggaaowmid.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gzrxgebhn.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gtxgocfux.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gdglpewas.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gbwwgkxfp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/ghzpqcyel.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gisotrqku.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/geppwtqre.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gawozgdee.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gfsrxjajo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gejqdxsfk.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbminptjy.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gdyuvesal.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/guyqvhbec.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkwlthjvk.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gduuoucww.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gitcfmnsn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gnlbvvmxe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gwxfomvdv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/ggfdhxibq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gznnfkdux.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gonkkztbd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/goouejigl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gejgubjrg.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gkencbjen.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gcxfrbmli.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjgphvqg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gwswopfcy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/glmbyxnqp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gklvsqxtq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/grtsjrecs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gzlujwxnx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gnstabwtg.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gaumsffqq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gvvixypzr.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gkhsfwlho.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gqddaizck.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gxksaeknl.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmwirxfkf.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gdwodvucl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gicpidazs.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gebyenalf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gthhbhjlw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gbekrarpp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gacnjmqfe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/grmazdrxp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gvjqvwbbu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gowpgywrg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gppycigeu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gixudtuij.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gohetledj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtmqskuzf.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gqbkttgdu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gezqcqhro.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/goctofdlx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gjjzvmswh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gpsfkrkde.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gkrozjacj.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjjdhocmj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/glzfyhsnf.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gxkcqofku.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gzdizufgr.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gcldyuzkn.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhpchni.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gszijfrpk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gxgxvxypc.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gxuhglxzb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gbzmbovkc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/glizaaxfp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/grwwitxum.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gezdsikdc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gxhjisswu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/goqltcuwv.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gywdcgchh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gdszhpoul.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gptlfhvzc.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/grpppbttb.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gvgxbmokt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gtgoihsgd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gdlhchufq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gidppncyk.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gjfamokoz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gtguhakbp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gkxsfxooj.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gvykbnzwg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gfjszfygh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gqabgittc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/getxlvsxq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gsspsolzx.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/grmovluud.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gfmctxahm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gcthqgyec.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gnvlwhepw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gqxteupzc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gxewczffy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gggvcrkjg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/grdcriznb.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gdzzmlpwe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gfrzxtvzm.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gpvqjusnh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gqqfzwmll.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/ggkcfkeea.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gzshzgubz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gjdlyaqja.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gjcbfzthk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gmjszkxhx.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/grqiaazxu.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gnyptiozt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpyikrgww.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gqaivbtio.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gphptujer.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/grjodmzak.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gsraigotq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gbakaoqnq.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gvfpcpbcz.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gaskzeefm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gahttzuwh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gbvmdzhpv.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gxwqhsjcz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gytwxxuiq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gzkuyozau.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/glajvlohw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gjqnftruk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gqmpybppz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gimzfpdzx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gbrxjvyqo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gsdrifvvf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwitejqkc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gpsczxdyr.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gttdtqabd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gvevjgxoo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gghtdfmgh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/glvvjzdgp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gslvzondh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gwinmuwld.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gvvlvnmyl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/glfyjjhjk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gtbwnsvof.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gzxqrpozf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gxjwqpjfg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gsskfiatu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gqdfptcdo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gmwptdrsa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gfackwldn.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gyocvpsxt.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gyhvinpkx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/grchtykgi.sHtML


<!-- 参考信息 -->