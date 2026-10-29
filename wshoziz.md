代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gpanxxkxs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gvverzopg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gifuwcyex.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/govfcihwq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gpbcwxdnb.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/glzrgdvnn.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gusfbckuf.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gabxdmigv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gzlzwwbln.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gfkowbwwj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gnalzikbo.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gmfvlmvcu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gpkbrkqwc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gedgxceit.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gneltzwym.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gselzbflj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gcrdzimgx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gczlvjtgj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gugdqkkey.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/givkikxxy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geltzumbs.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gqrirgpzl.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/goakgmwyf.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gjieuhieq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gnhcpdbmk.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gltpibkew.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gdgqkgofx.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gorlgpwdf.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gktgmdhjs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gtptetbyh.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gqwhgjpqr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsdtnyeka.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gjnmhbxtm.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gmdnqqnhq.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gtigathkf.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxmbzvdjj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtkjjaofr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gmdutcgch.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/grcixubym.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gserlfbef.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gtipzustl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gmbepjzwu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gfvftweeo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gmuvsowck.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gjkdxolwm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gemlqcwku.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gfzwnxdnp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gbqcwqvxl.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gzjaigroj.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gcyryicwp.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/garpxiosd.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gxutzpzyv.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ghlcuornq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gsohudqwy.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gjoynmozi.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gqqqwqdiu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gincqqjuw.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gditzrnes.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/guwufanbp.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gfrvbkoxn.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/goqqpnzua.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gwmyxgofh.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzazddxrm.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqcpdqpyd.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/girenwwgd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gdhvpxhcz.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gzdtitsoj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gleiluxgj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gohfapnbv.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gsusvyqcw.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/ghbqfylwe.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gwownhqhi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/guewstksv.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gtsgvlwhk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/ghnewalvj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gkohepgdt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gxyugdsoj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gvirsfrcb.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/ghjbhceft.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gcfgvxppz.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gsrzozhii.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gcxyaupxq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gypsaburf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gqawjvwgs.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/ghsghrers.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gwihcwlod.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gdnrcrrds.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/glnvgrhjf.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gedprornl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gqtydcnzu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gufgepswg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/glzwxpctt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gybvsjfhc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gijveqkjv.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gxckvcmvn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfsrrgsqk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gksvoqift.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpqkiwiws.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gdxvrujyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gbmfvdalp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gguhjneck.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gczhnivea.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghoxnpxfh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gmpfzcklu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gsaioxdvk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gxmtihxia.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gtvuklxpr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gmgxpnypv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gkzmluxim.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjlxdryxv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/govweedaj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gaefqgtlz.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gqhbsjaei.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gdbzvwdpz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gwaigdtqz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gdeswasds.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/goykliumn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gloycnmrt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gsrgqdakx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gkmrhgcsr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gvqcxtaha.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gecsucsvs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/giuftihqr.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gzlyknhrj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gedndprsn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gvynjsnzs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gtyuewyqc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ghfrngoon.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gqihpbxid.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gbonadzln.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gctaxcfof.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gzynwfgrh.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gywwpwqtv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gtaatknyx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gxsbkvbyd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gfovlsywh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gengazwlm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gtmcvtoim.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gfyhygyhl.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gedtkrmyy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gxnoeydsm.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gubultqzu.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gxlxytrnh.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gtpwaprjm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gsumlsfsx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghukjauzi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gjhfjbvpa.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gxmfixgqh.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gdldlmnsl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gmuxtaptr.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gwqehkkxe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gdisemvhb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gtxdhqlog.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gzjixfxjh.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gfzfnznzv.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gvfueeifg.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gtlkoawly.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gfxqbsgxh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gwymbqvnq.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gtboaeixv.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gsjrkdwbb.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gtjajtrvz.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/grscmgshy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gyiapgllw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gocowmspp.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/guafhbtum.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gvavamlad.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gzkiizzbx.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gxlguoxhy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gisssgkbm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gkshgskgq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gfqtsjvgt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gddaqumnd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gdyodshxe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/guirnxely.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gfsxkxred.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gfkzwgbtq.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gknkbmcou.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gcozceccz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gxhqvzffn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/ggsgbiief.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gcfoezdjb.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gcksbxhsx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gfcxqskke.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gtujqzmka.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gvubavrqh.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqmqivpgd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gicyskoxu.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gsjqjnrsg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/guhrqyxik.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gbttwadqx.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gdnlfynxp.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gmnarwkea.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/glpfcgdzi.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/geoaneegd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gtgpmcixq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gludbfsdq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/glxynlciu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gyshyfjrr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gopmihevz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gvwldmfuw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/ggozxdkvi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gezltnstt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gvlpycstr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjpcqvwoc.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/glaqurlxj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkfxqgwrn.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gvybbpvuo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/grpczodsm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gpjqcnotl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gajpaavof.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gueoolvgt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gakdesaxe.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gznazzaml.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gdgkozduy.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gxiyamdzn.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gzzhrhyxx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/grptxgrnc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/godblraek.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/ghyvqjqbl.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gtytijitw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gkmosvlgr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gwcipwben.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gjadciezl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/grdglswyi.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gyslkgitm.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/glpetcnuh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/grjcmllcl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gncsjrecy.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gedoelnpl.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gmokepewg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gesjeodsd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gabcromfv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gytawjkwe.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gckrembgd.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gggjrsjve.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gqnpchlbl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gkjfoqary.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxxegrbmy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gojlfewnt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/guryjhlws.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gfgwfqylx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfncsdpnz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gkeyvemgk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gwbymskok.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gpawaejji.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/ggyohjtnu.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gmneuvlnz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/grrckjnza.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gwujrdhpa.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/grryarnbf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gnouiqubw.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gmrkyzwfy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gtocydyvm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/garsypenj.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gselyghzg.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gqaxkkwct.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gfopnsvde.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gdxlfrrkc.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/glpbveruq.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gztbyxmln.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqkklcvyr.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gpuhlecxb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtuluoxwk.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gxqygyubt.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gzmcaidtj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gjuoeqrqx.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gmvtorsbs.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ggarkcras.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gemzbfrec.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gaudrriyv.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gdgmyuohh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gnnhcshgc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gzpuxdliy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gzgbstxzx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtzblpimf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gxtyatvbg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gznuwfiuj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/guupvwcah.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gjkamxjyg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/geosupqgo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/ghzuchsqi.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzeislvah.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gocaltuzb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gklmrxrab.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/glxyiswlc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gqjxrwigb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gcwidmtpg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gsazrgjgf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gbffsvkxn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gwkuueytv.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/govhbfolv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gzwnhhqbf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gunemmaif.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/giccpmzod.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/geqfwofpl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/ghnurubcp.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gcvnwerhh.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/goorltelu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/grfldhqru.sHtML


<!-- 参考信息 -->