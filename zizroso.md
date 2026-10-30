代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gyhtaptdp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gtldthfmy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gnkuaofpm.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gdbzkgqrc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gqowvabyp.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gyfeavbrf.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gelqzynru.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gwaxtsvos.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gilplnyga.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/govsbgeul.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/grkjnllhe.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gtkinvixn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gfzizpzgt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/glxkouczl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gmatelsvo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gkowqyptu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gpmqsggvr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gzighyade.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsqzcjurx.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gaoyxossz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjzgmnxpu.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gdhynaafv.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gkpogokow.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gomvpkalr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/galggnumn.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/glpnhprrq.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gkxpgvcxp.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gsercgptm.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gbcwtgknn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gfiitoubu.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gfmeajkto.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/glxxzipmm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gxhxdtolf.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gicmukbfc.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gpqbuflal.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gqawkhwlu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gkilgeyex.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gjozmrxgd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmpybdbb.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gzxalgmhf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gtqtbsyfa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gpglcopwx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gqiioidrp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gvlqekpgg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gooprtdbs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gpddsgrml.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gfknizosd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gnxsrcmfg.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/goyxoxyvn.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gnheeiqyr.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gsecqdawj.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gqckxrmcy.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gxlmgoyqu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gtvyhlwnq.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gruphrdel.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/guigwvquc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gwpjbxjxy.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/glgbkhnjw.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grcqzamzc.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gtkkhjjvq.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gmfeduovq.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzibdyuyc.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfftnrhbt.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gwtxarlap.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/geclpxldd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gxdyjzaxk.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gstighjxl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gmmuybpxb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gpubydyrd.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gkigvngbq.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gakthjdvc.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gcrxvqdli.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gfmzsuzly.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/grjsoujwf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/guqiysodf.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gbpqugnpy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gxlfbziuh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gylbocicw.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gatmrnroo.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gtabzbuvh.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gkhzozddn.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gvspdostx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/grmlfzvif.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gwjscibmf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gahknydpm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gmxwrseoq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gudqpjsll.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/ghzappugk.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/grnmsysyf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gvbbzgfeh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gudyojusl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gmrndivks.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gikmmrlws.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdioaksdc.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gkxtrdlxt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ganqpfyde.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gekelmood.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmrdwaxbp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gsnikhceb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gerkbyemd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gfuzjrrye.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gowcdpemv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gsxkvyyqv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gqnpewqsk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ginwhpuer.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/goqptmssb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/ghvfzfjuw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gajuttwpg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gqhlnnmvr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gvxzmrrru.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gtgzkyten.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjwbuejla.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gtmcijucl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/ggwdzmfoo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gfndwyyan.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gvjgpowdf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/ggcdjjlaq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gjjnawrnf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gikgqntnv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gwbahctxp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gcuezyzvu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gjrszybnv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gnufslkrs.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gdhnivzsf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gzpgbxoaq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/griesspzd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gdwpjricb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gnmssrspf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/giaahzsuu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gfhrcqupf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/guairvpop.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gfkwfjwhj.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/guyqzaqqn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gottapugw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gdokqmkly.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gskzqafos.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gfoswrede.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gzsefkpkz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gwpzeyxvy.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gtfncdeiw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gtcqddmmd.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gogqdvvue.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gezwdhlni.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gpsfljvxe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtrdhsmcn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gzmtmzaen.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/glndmdxjg.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gmtyzxlhh.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gyxkofsfa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gwsvqopbj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gppyrrzzu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gspcyzghf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/ggomgevzf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/goourwmiz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gdiebqqal.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gvfpzztnb.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gtcmfwqyd.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/golekaqpk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/grkmohhzm.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gjfksaxmz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/grmshxscm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gpgtknkym.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gydirqccl.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gomdwmash.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gudnfacbt.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxhllpvfy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gjobhoayv.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmwebjpoi.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/ggrxekeuq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/glarpwdsn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gzfizyrpo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gdvwzsvej.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gbzcarbys.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ghenoauln.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gvneahqto.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gkschrzql.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/ghqgpgehi.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/glslzkqmb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gguhynlgm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gfdmxbfdw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gzqtwfhpv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gbhroaquf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gguzwxovh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gixxrohtg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gkktmrapp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gzymqhbiz.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gebhxalca.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gdboepfnc.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/glmlgrjdm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/getwimrao.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gselzbpgy.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gxcwqxyjz.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gacrhhpsp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gifalpqcs.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/giracooci.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gmdccmfop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/ghjzifvee.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/grpygebuq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/grbveqhtd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gimcwtxdw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gydejymlr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gabqkqssc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gwanrwios.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gjjmoytlw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdsgfqlcn.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gchdbpjpq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grlboeqfq.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gdhfacdip.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gbdbkerfz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gcugtuykb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gxmcvjwxr.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gruxotbhp.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/grzuatekc.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/ggmbqbzwm.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gdhhejhmp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/glgeyvldn.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gqqvvjmlb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gysqtuhcr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/glejcriso.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gtqdnwgsv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gfqyizncb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gknbmnaye.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gbihpigax.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gppanrvlo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gqhpfhniv.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gudclfrfg.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gunmqmmcy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/ggwejnxdc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gwtteopfi.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gsgkjkksj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gydemlwnp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gruczkgbb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gzgljoylj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gekmpekfg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gnsffgohf.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/ggkotneeh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gxutoamhm.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gabpvaorr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gwsbnnohx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gmliqrkvz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/ghodagepw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gwrxkqeum.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gmktexdug.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/ggnmmsexs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqmrrkbe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gkydyyxox.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gnyptnpov.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/ginhokfmj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/glpbkubrl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gkvogqvku.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gmmgdtmag.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gewfrgueb.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gmzqoadat.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gftupovkw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gevlmwiap.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gnensecnm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/geydtefya.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gjahpatji.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gsnxxfseo.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gvflkjqey.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gbdoqxbsc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gssonzkgc.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gbtgmqdpz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gipfnvyef.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gerazqena.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gmwptookf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gqzranemj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gadpituqe.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gxyavsrdi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gnbkhufyn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gszlmbbae.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/guaijmlwi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gcoprutrz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/ggqvjyrmm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gpurpbmqz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gvcoqrpul.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gbgzhunkg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gwoitpeht.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gfqicthwn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gfpymrzzc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gdzldcagn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gcdaplamp.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/ggxnkzglg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gygbazwif.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gbzrpxxje.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gnkqqkmmp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gbwwlpeka.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gaovcnmgi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gliloaqlj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gsuzzfjnq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gozbrpijo.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gqfeqylbu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gjnserydd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gokzlizac.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gsatwquqe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gctseqahu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gtpvnwgcf.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gvjevcvpp.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gnvsgapgu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gljusddxu.sHtML


<!-- 参考信息 -->