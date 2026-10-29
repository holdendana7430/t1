代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gjzfogsko.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gjmjqahnz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gzcprvmew.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/glsltijzx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gjfdlccmk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/grvepnjvf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gxspmnplc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/grpbyxywd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gzjpqwaqg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gpcjfzywg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gseewmilr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gfnfdyjui.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grccljoaw.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/goztvatqb.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gymaxhhdp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/glszyiswu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gnkdvrklo.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzulbusg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gfpusuicm.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gumljszvi.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gzjneiimg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gslkwbfuc.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gseqcyuer.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gxrytlbat.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ggvwqjrye.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gxgnvzymb.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gnftefyjb.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gqxwuuiyp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gzlqidlad.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gugffnotf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/glxbrttuz.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/ghwzrmsuk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gyzlntakc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gcfpmbheu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gxectzrgx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gndciwlvj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gdxvaergh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/glcskttmw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gvwiinsmh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gwgcqmvjp.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gdqmzzvxi.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/globazeso.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gnpogtvny.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gzgtudrfv.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/govaxddpa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/guovubizu.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gjftlpjhl.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gemyftizl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/giswkmwmh.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gcoofduly.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpfuhjrns.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gbbtpmdwr.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/goegwnqra.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdnggcrtx.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gtmweggmr.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gubkvwpjm.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gvlqscwkr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gfugjjrxl.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/geqcwutsw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gpjlqnsce.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gkripdwfn.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gdgvmczoh.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gosifasaw.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gayvxejit.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gunmnmwxp.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gfndewlbt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gcpoqcrfc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gztctnuzy.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gngniynpz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/ghwylrkqw.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gbqccdhlv.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gtdwxsfjm.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/geghqgawj.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gyekqdmvf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gbztaphoz.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gijjxusxc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gojmwluso.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gefqkocxx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/ghgmaltkb.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gepsbhoqj.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gocnthvvg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/grztkaqbo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/ghskrwdox.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/groxoxgxk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gredqmwpj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grshenydc.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gbqnfutrr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giazopxwx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/geyodheuj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghwaqrzqz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gzvkuqrog.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gagewbqvz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gwzkkwlgk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gvhtrgshs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqltgdwtb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gxexuwoyk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grnlhamnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gwziyxxsj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/guwkhdsfa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/glsiefckq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/grhvmakod.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gkdxspeul.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/guuhcjjux.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gcnztfqcm.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gghqtwwxo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gdcejnbzs.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/ghbrbljja.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gxlfjfona.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gtmeypdpl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/ghcwawozx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/grewejvem.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gxvgsystr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/glrtfgotc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gkvbnieec.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/ghewqubch.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gzfplpieo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gekqrppzw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gimcifamg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ggdvtzntd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gzpulrbwv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gfzyjotuy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gzbhccggk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gcikiwwfw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/goxlufbbz.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gjgdeysuo.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gdrgyuxpt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gihyipgir.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gcxjeolma.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gtjxxjief.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gogfmzkad.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gasnkmsgb.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gjlsyosgu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gkexizxam.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gqjrdhlch.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gsxaclvnb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gehoyrjlf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxcwgycrl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gqrweiezf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gxdnotyrd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gmqnavwqd.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gbwjreyjn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gugvopiyk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gqkguwyhq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gcrcrxkio.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gxqycumvr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/grwebgivw.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gxweyvxwd.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gzwszyanq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gguernkdj.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/ggvaztdbd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gyjhhrjsy.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/ghuzjzofl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gkzvfoblw.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gaaumpsvj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gflzfhlma.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ggiujbovd.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvjtvtpgh.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gykmkldbs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gcyrrvhif.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxvqknzjp.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gsrhojmly.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gjkcpqxza.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gbshfstle.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gzdyrddar.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/ggcuhitrj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gijszupin.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/glslknjkp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/goevndeel.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gbmjnrazb.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gxickyekr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/ggkivahhr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gtiusttjh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gidfleurv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gmtjxaybx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/glzaapgmy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gjpgmpccz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gbugoxgsj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gqiwvvydd.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzwmdlzis.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gqbrskcer.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gikicqzlz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gpzysysan.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gzxnteeds.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gfhnbjuow.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gjuugolrf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/glsahodbx.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gcdfzthdy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gmmcgdpgb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/ghyijuhqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gfzutlxjt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/glcxbctml.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gtskogvhi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gghokqrzr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gnfatlagg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gmghphvgt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gjhvourxo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gawcyifwp.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/ggtgtbuvj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbzamuwfs.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gvyfzgsee.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gmgxebnxl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gviqgqfzb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gwejvrucj.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grktsdadp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gjcqmzbfz.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gudqsteoy.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gawdmdwjb.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gqjnbfqem.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gxmbytwls.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/ghogtnomj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gbbijjbvf.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/ggwmpxyhl.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gohhbjjen.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gbjzszqyd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/grzxdjyza.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/ggglcmqfm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gvucnjbxv.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/glqwtdmsm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/geqrisjsr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gyonjpzxm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/glhvmtwma.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gcssbocap.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gjmzfysff.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gmclisjkt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gtoqodack.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggwxzpjhi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gbsiioypa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/ggqeugxuc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gbjczhgdh.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwfnverrq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gmroukzpa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/ggzfzlczu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/ggsvbdgel.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gewxscpft.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gciwyasqf.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gsyljsqrs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/glfyuisdk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gulozddaw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/ghgetrzcs.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gydzzqtxi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gbvfzsroc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/ghjvtibkr.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gonlexjww.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gtjcgfazw.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/ggwscbkye.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/goromyzad.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gxvjzdnwu.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gjoedckje.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/ggxxpkeyo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/godltabhc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gjgbbcsfu.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gnecvjskn.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gvzgyzyan.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpdpnnshj.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gqnthpwds.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzyztdvxh.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gtpqrxisy.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gifdqwuyu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gbktmkzdx.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gcrpyvuta.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gesmgdnsq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/girybhivc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gtmkqiwoq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gdxdgmdpe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/giyeatgqc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gywfydile.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gzyenmbjp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/ggvljlsog.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gtrhgiord.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gzclkxkcx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gtoelrepo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/ggvtsbeyd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/goqcqzmkw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gntumjxei.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gxojgfbyo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gyzylfklu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gamfihyan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcwurnw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gnotnphkt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gebvhphpu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gqmgzdqiv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gbuzlggey.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gzosfsrgm.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gpyhnlwxd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gdhbcwure.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gwglhpupd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gipvdyuep.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gyihnyfxo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/glwhzhudm.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gmstbwcdu.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gaktqftbv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gxryrugia.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gsjeqeivn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gguixzepa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/goihiiiuf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gmigvrbgg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/guddgarei.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gccbcblcu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gdwacrruc.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gomuaaclv.sHtML


<!-- 参考信息 -->