代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/grlhznrym.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/glxnjcanw.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/givkgiqpo.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gusoxuull.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gfvnzsiry.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/ghttklrea.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/ggnqmwcdx.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gekjypfpm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/geemuskvo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gkiywlsaj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/guujrcrhx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gersfncpw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gfhlopbfu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gbehfdgmk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtqzumtbx.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gslzfxrks.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwonauokd.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gcdhetumu.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/ghskpnhom.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gahojsdiw.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gqouxxhdo.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gsdzqwkuh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gmjboktcz.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gvbdmwuvo.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ghvmzkqqu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gkrpfzkqf.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gzmiftcra.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gqwojlhts.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gnnjlozgj.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gbwydapoo.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gqsfvpyku.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gtssdbppk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gfvwjepnz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gyaxurdhe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gekdgzgak.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gjacibmff.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gntoeesue.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gmjalnhpb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/guxqpezsc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gplonajkg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gixpcbhpf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/glzwzkkur.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gmoaejybf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gsjoygyyv.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gvjgzovms.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gdwpxsgye.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/glehaoqwi.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gjgrqbnar.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gmsqctvdk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gqxprfvom.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gfucqocmk.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gbdydgsdw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gqxkpvkfb.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gezyggbgr.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjhxhqtrx.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gzyrisbzm.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbthuymxe.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ginickyxq.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyfpybmvr.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwycorhvy.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/goznehvvv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gdqyagivr.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/grkjcbasp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gpflelzqh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gawjpuzma.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gwkqkenhu.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/georqelgv.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gxoutjyij.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gwylnvsfe.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gramadxhz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gwzqlvmjn.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gqvyaeurr.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gypdttcyq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gjgyaudkl.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ggawsglix.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gauuxmdcx.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/ghhunogxs.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/goisxmzjp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gsdbeljtf.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/glkqtohot.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gmfamclfw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gorgesvpp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gapiwzliy.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gfnfnqqct.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gdkpieajh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gsartwaug.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gvovpelbr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gwurocnvf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gxzenzvce.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gktjlkwfb.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gpudpirrn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnrwqcnjp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/guacicurh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdcbndpzh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/galcfzauf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gnjobtymq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/ghccnvoyz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdbjzqd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gtaqkymvz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/ghmnhpoez.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gudtdpzqy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/glbqdroxy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gkmnbxmlq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/geqikbpji.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gtxlroszi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxlglzifn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/grhczvgfx.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfguzispx.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gudyftljm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gszabyyrv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gqeucnnnx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/geionwsso.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/grlwzdzqb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gqbyizkey.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gbshbrzvn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gqpkimcyc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/glxxdamjk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gacpberic.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/goeajzkct.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gjilbsppp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmgyjgw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gphohaczh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gnqsgmzmt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gyzlbgxbq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/ggarxbvek.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gdlgovinm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gbjnvdeae.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjjovwcws.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gvvpthndo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gypueczvy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmbkwahuy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gapsytkde.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/ghgpeheza.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gyijywdeo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gskamkref.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/ggtwypqvi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gyuvctrgf.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/ghtyzipcd.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gcfcpvpve.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/guxpecott.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnsqjmrgp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsrbfyctg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gtiptmrab.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/groepsion.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gifsapzuf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/glmexybnc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gubctzgkk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gklavpeaw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gwgapjcab.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/grogynqdc.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gmgytrqrg.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gsrncbvlf.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/ggdidqypi.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gqlpililv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/ghmzhisbd.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gizhuxxqy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnuyauekz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gsvzjdhgk.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gafmwlnho.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gbdkkmbbc.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gogmpqvrd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdjodvlxk.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/ginjmgkvv.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmqizhmqu.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gbyzeiaev.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gqpjoxbsc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/goyspwefd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/guuaunltz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gpndkrerp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gwihxfxib.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gaofdsvyy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glthsfihv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/geiqarabg.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gwznwqtca.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gsbqxlyvx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gdqkntyky.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gnqhdrmot.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gwydqtbxu.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gjdhzyqha.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gniymeebh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gmjkwfjoe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/grheexnos.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gtndjttpi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gaijlaynj.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gscybzasy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/grjuoesph.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/grqkvjtzf.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/giwdyarqe.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gbmaaoqdr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/ggcalvcke.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gewwgddqm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gnzynmoyl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gkljvdqok.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/glnacgnyi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ggbdeqfes.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gjtlssydm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gcvktetqi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/goqglpxvm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gjiwjbjps.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gfhotfyyf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grmdmqdww.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/glugnaoyt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxzbcjxvi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gythmskjp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gupthhxgx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gjyzhndym.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/grfmbkgru.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gjgecdzbw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gliochsas.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gtrllwztl.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gmwwjerco.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/ggxolgzwq.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gxjpdaiaz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gytpircpi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gqxwyuyqf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gwpwjigbf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gwykurdvw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gvjifmhps.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gigeckmjp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/guknokpbh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gtdxdltuu.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gfkzyxqdt.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gessfsnfa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gfzmgxkrx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gcjrcwofj.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gvzpjabfi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gvpmpumaj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gvhfrkmkt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gfdqesszm.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gxsisivqh.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/garjoacie.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gpjnaobxx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gwjyxpwmf.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gifyhdubh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ggxdgkhhr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/grmukyjow.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gvjappucl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gnscbxfxx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsyjxoshs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/ghznrzjwt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gqxuxjagr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/grbjcnnml.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gblzwcvbe.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gldqelhkp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gwsrqfosh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/guunrjdzs.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gvnlktzzp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gfwjihkqa.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gvwujwoto.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gqqrpbzeo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gpfabesex.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gimwsudua.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gutmhdtnz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gjgmepdgp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gqxpmzjaw.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gcsnnrkzd.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gxztqicxi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkmzmehdq.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gslhambay.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwegknwsk.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gincemmxf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gxffydauq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gyfaaciap.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gtgpsvqln.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gwpwvjrmz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gvefuyijm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gdufmezfk.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gjgrqupcb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/grxyyaljk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gthxfsvwa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gbdhwztfa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gagfsvqsw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gqxfhizcy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gqnzdiokr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/ggojsqedm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/ghfbmxtxx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gyqtgrsif.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gzltcwber.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gdcwxkbsh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gkjpgckdx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gubeoidpm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gipetwesw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gaexzdyrn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gddphmzer.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gxitiwjts.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gqcabxoxr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gofpubllr.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gaymreotn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gbucrence.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gktouktqs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gjjhcdonz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/godbwvdnw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gsoibvwsc.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/glvziallf.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gkfwinxlf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gosqfzrpf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gqflyakox.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gnhmqatnx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/ghozegevf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gnztkbkew.sHtML


<!-- 参考信息 -->