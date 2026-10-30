代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gzqhhwxhp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gfijcobrn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gfaaefeoy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gqcrcndxp.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gtsiiittl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gxlefhmyo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gqxkjgpmu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/guxopufpx.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gqbbvqqet.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/giveezwoe.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gvhkqwffz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gvsoyahpg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gldxexlzs.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gaumhljdm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gzqhzetod.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/guazrazcm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gsmuadgvy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gmgccckdw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gnpdoujtm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/glgtzrsvt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/ginrnbgnf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gqeejiwgf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glsijihbl.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gquwcqgfh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfeilevgn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/genhuitsb.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gnkqxvlvi.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gkinzpjss.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gnqhmxttq.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gokttujmf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gmodtmign.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gtpgliwxw.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gqdboweux.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gpoxurkwp.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ggrrcmxhm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxyozagel.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gtufnoxcb.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ggxlgjbqe.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gjgxawlnh.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gzcqfurco.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gatujqkhn.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gsegevote.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gviyqcmvd.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gimtkprsl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gkusvrmnl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gviezjyps.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gwhdoexow.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/glqbjaeuc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gbuqrqvgm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gxlctcvmh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/grerpwrxa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/ghaqukpax.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/geklkkalb.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gyjnplzmv.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gsripcmfe.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gcvokwfgk.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfjpkebxy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gaolvkwpb.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gitrlnecp.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gnmgluivr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gdmlfwqzf.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/goyknizyq.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdrnlnwgf.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gaehaukmn.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gnpnjdvmt.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxsrkoymq.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gsoupewob.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzljvedeg.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gjhtpvrzc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/giwaikyue.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/glbjmunnh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gvkkaxhjd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gaxxezwvd.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gbawiylcy.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gbeeyrble.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gzxyxgdie.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gscarlfrw.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/ghbjmjvwx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gyuawrakz.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/guxmvdlle.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gnvpogmjc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/ghvvbfsvq.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gxuxqxlob.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gpbbcayva.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gqtnozhtr.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gxuszlcvw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gqwicjvmk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gtlloyuzx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gyjpwqgxd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gvmjjctte.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/ggqmylyrn.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ghsfiyqxc.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gxcupknqa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gqpiofvob.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gmezyuurk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gayjzqdur.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/ggxuxpwbg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwrqmpsyw.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gbyxewjul.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvgpoxttr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gijxqmcat.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gskowaprg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gilvdtnvv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gsybyfsci.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gckofddoa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghbacupwt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkutsadyk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gazplclvf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwlusnyni.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gegnyibmk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gizlftxge.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/grhlkjqom.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gnylraybx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gcbaxpjqq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gwxgsrygd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gkiyqqpmp.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gknvwleko.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gdovzxszi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gyswksmff.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gtfajvcbz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gtmreffdo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/geoxwdrey.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/ggtsrjgqb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/glvrzxzpr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gvlkdxgee.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gjgdzedqy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gxvtecjvj.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/guexvmgmc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gzefpszip.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gyoknusyd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ghiodhvjb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/guwpuvlrb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gytqrtmrg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gocvvtkie.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gmzughuco.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gfqqobgvn.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gbgnuqixc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gkokkcpnf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/ggglbqdis.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gmmauvnti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gnhwigmzv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/grvwpxrgb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/glfiqmwkt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gzzojxfvu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gptpnwxie.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gnyylflzv.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gdgsvsvwz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glsjweqqh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gckhsqhhc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gqmrwnjyy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/ghlxradaq.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gtcrdrfat.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gwirquhgy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gwowtjhhy.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gfeswicwp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gegcwbonh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/glgtapsvw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/guarlahab.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gtowwbijg.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gmshmoztf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/glzslnjmn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gyzjttajm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gpbgakmln.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gtzcnbeos.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghdoblbsc.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gmcswxiue.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/glhxajnet.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gpmkiosww.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzadaccsy.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gupbdwhwq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gsibxfvow.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gppceuayl.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gcpbzadnh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gktvadbek.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ggisbkxwt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gazmsuidp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gjxkrdwrc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gsxhxmnwc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gdnblzxfv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gxiteqjrt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gapgpfryf.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/graguaxca.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/glzxowvdh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gefnybfuz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gqijaxxda.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gbwgymwwd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gctortdqm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gbezhkidr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gotwkpgyk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gldcksilg.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gcibfdyis.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gmaplfblq.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gjufhvxkq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gtwaruqoq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gicnmmvhm.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gckxfecsv.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/glsscfidp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gyikttmeu.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/glfhaxowu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gmuahuoze.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gsuykoauq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gkmrsrnop.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/guifyhcjz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gjkxyzybv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gwukmnzwk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gjpegqyjb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjeclrqne.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gijvuemdy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtodzszyr.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gimowveea.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtbdhnijk.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gkuwdmbmk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gtpwqjoqp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gefbjwaiv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/giqdrpokz.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gtonhgcix.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gswrwqygn.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gvjswuahm.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gtdqdkxgp.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/ggsuqspqx.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gltsxwkff.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gmujpwpnd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gsmuaowia.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gvfldgnzm.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gzsrlpljx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gjbdwpwhv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gmxburkrs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gaykymatz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/geoczyucj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gkegpvyck.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gaoptrlmp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/geylttbfd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gyjrdtnaj.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gquzlpaoh.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gkjbzjpmi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gxdumualr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/giteyzjog.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gxuvahoof.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gfscqzchd.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gazzrecah.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gpfmwberq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gwoejkuhe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gtgxzxkgy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gwzsdrkgr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gqsmdrvjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gkuiauqpw.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gekmuuker.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gtnpptkyw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gxwgfuxtw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gramjothy.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gknybrgfh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gqnxtlhps.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gdgznijyz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gluxzcxgr.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/glnprnmvr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gpeiebmxe.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gugdkyygl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gmptfvxfv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gdywngqsm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ggcayhgck.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gmdbmzcjd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gujpfcqlg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gdxtmoxbb.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/ggfcsuxqo.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gkgxmtyex.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gafudpqzk.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gegtsnjql.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfbxggaqv.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gbgtubzdl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gginojpds.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gemajrggw.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gdtcqabiu.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gqwhjuoti.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/grwabwzfc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/goeveflzi.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/grzyvmxlm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gdhakdkbj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gyitdwnxo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gonbvmvyr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gjldrxvec.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gllncmlzt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gvjqumhwg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/glojzjrut.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gvlqppsze.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gflyvvgsh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/glmufewro.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gguidmpas.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gojaywyft.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/ggthgizrc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gtkngcubj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gsdehhjsg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gwrhiyiai.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gdbmzegzn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gyjxtabps.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gehdlfbee.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gdzwhshuf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/grnhqjsyz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtsljnvrb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/guhehsegt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gqqcukeiq.sHtML


<!-- 参考信息 -->