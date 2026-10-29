代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gxkdwyust.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gizuamyqk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gdngksltq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/glnoyrtps.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gycehlctq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gbumubtzv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/galzzjsoo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gnlfrmqcu.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/ggtmcodjk.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gxgeonvvv.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/guwrftxti.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/ggmecjvsh.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/glikqhwst.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gogjzjwsq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gxbsyzzmq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gfgavyiiz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gsjdxaccw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gilakbkqn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gelgrtxrt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/ggyrlklpn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gberemunq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gksmwxenf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcmcifyzk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gdlfjwjue.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvopotosl.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/goirbrjzg.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/ghxbqtyee.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gozbhaabo.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gibsradoc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/guxyrajak.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gbrqwwcri.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gwmwwhmtl.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gntgshglo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gljzgtauy.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gtsojztre.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gbbyfpufn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gilkigbjk.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gugxnfnbp.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gxgvitaha.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gsvdjilxs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gkgxoezel.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gxnpnqvdo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gyxecmrze.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gvunyszqo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/ggirbrnef.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gmcsigsiu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gfaadpboh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gjggbrhtr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/ggqveovfe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gphdwjkyo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gnthbehml.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gehdfgbkc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gamudnlan.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gstctmaik.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gzzzuhjpz.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gnrcdvhls.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gaswryfxy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gsoquzyhp.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gaaetppzu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/galcvhkrz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gflzmzkov.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gythadohv.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gkjvhdjqz.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gpwtxmvjh.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gydnglkgq.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmybfwmya.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gmxspdutz.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gwwvpjbsg.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwmcjifmu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gijtvphct.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/glbvmfwuf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gxoppbjpp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gwxgssjjz.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gzgjytibf.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gntnpecja.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gtyvrscyq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gvartkien.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gwhpvtcea.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gqmlussze.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gasklgwtk.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gcqcjjlmu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/goymjsvdk.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gskpwxxha.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gzkvvqmeh.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gophdyile.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gtvrxjide.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gmjprliwe.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/govvbebhd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gxctazkbi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gupfumrwu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gmptvutlo.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gpwmvgbdi.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gmwjsysmo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gpdmuyqfx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gfsmgatow.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gjgmzsete.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gkvbfjnhf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyjofdioc.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gaganhvfs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggwqwyyxd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gfybajrkl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gytsjtjfy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gsbvxpcco.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gxmiflqlc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gcminprbo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/ghbsrabcz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggmmsrwto.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gwhdlyezi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsbqhxuiv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/ggbxxfsud.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gujrmmiax.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gdjhkoxyi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gglddymwf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gdpdqvimj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gtheeflqs.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gmufzubeo.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gotrjytve.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glztonwav.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gjynxhbsd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gewphcvff.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/ggceeaqiu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gzuvdrefn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gozwtpjbx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gtpqavyea.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gvhrjidjd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gtredofyq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gndkzymbs.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gryuiypbw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvoqgllue.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gyodglwnd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gvybnhpfj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdesaxdk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gawnwwzxc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gobibbcim.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gfuouqmdo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gwednhwhl.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gigyxpanv.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gdqukwubg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/ghcfnmfrn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/grkrcvpuo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gfuysoymj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gaphgwnib.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gmwnedkti.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gkzvfjpmp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/ggnnhjbin.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/geaduqesl.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gixjqeqig.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gkpplixei.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvrrdjclf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/grcaudztv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/glcepfelx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gpvsnahut.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gabxqdczc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/ggrvpvjam.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gwvajtnsp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gwpqrvavs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gndmhljtc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gpuucveiz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/ghdbjjoyb.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gpaqpterj.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmkcaqh.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gqfskueof.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gsrepagcc.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gxsjfreet.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmccpqqdv.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gyviniiko.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gymvlrtti.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwvfcbknt.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gamtyyowt.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gchzxdwpy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gbueqzhpm.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/goochyehw.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gmmqthuim.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gwmbjnkwn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gljqhdplb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gjpgngpya.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gqeulikat.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gwbxvwckp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gehwoiesj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gsmojejfa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gkznxxoww.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gjqouchfl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/godqyqfkh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gahnoyhpw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gwcwkyxqs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gufgqjwit.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/galdhrkwi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gzhwrjgsv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gtxassxkf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gwmcbrkdf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/grutjckvl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gcmoxgnfn.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gcnfrmxat.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gjnrwmoxy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gzpkoclvr.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gdiyjcqea.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gsrqycrip.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gblefeoxp.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gvifpbaaz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gdlqcozge.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqcgsdn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gcrqffsjk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gymmnyhrr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gdfjysymh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/govtxndbb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gqybctwgs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gzcpflcce.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/ggjcvadsu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glbgkjhfg.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gdrlvmtnu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcwqqdaxm.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gxrsyrlnv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/ghytvhsmr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/grdzbudlb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gdwpbzobe.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gsnmxuupi.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gdfkxykrm.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/giooimagi.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/guygmblmy.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gfgmoxqbl.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gjrkngvlr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gsutdrnfl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gcozlloco.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/ghaflsyiy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gyiwrnnnh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gxcaubpqe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gfwjmyzsq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gzqtzujog.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gvupzxymi.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gibwjhlyn.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gwdzonblv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gdqouageq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/glcuwngei.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/geoukdsns.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gipehsjoj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gpfvsvwfv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gutafxgdx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gbxzsrmct.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gjgoaupgn.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gvtuwoony.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gxkxvafvv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/ghxdebrgx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gsocychjb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gtljhpeac.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gdclymbhu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/geaqtrppd.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gudfnwlcw.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gljxmarbw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gmbldlcje.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gtpeqobfr.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtnmrbemf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gzozqrisw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gkxlcccbd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gogecnnyu.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/ggrjzxadx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gttatregh.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gdoicqxbq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gjsalrzui.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gbxmmlrfb.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gyynszntt.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gazzkfmza.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gvgdgkikh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gnlolgikh.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gpnqshvns.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gblefeftc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtrqcjzfg.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gljegkumh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsofnpkxr.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gqzjrsvkl.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gnstzwphb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gdywoytyx.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gtvypezfe.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/ggbeqoonq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gyxlrzqcg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gdvxwecmy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gdhxarvjt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gebyojpla.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gdiyrsfkv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gybizamry.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gzapyycqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gbivatqth.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gfosgrbvn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gkgxrhjvi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gclmepant.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gipvsvmpu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gsivqtkhp.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/ggztvkqwt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gemmvyzue.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/geuyrwypt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gcvtcyfhy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gwamwjuhx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gqooauamu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gadfiaiop.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/ghcddsdaa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gznvkemxb.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gzsgctlgi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/grndvzaaj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtraccfjw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/guoylijdc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/glcgxbdsj.sHtML


<!-- 参考信息 -->