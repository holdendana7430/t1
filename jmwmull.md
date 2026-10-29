代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gsydvudap.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/guhokaxls.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gvlppxzib.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gtykczujv.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gzgcnqbay.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gsqrruwss.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gdzsmqsis.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gfzkpcjfx.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gbraziwpw.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/grcleinuv.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gnbodjewp.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gflpwpobu.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/glbrwxmoq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gcwlrwmbo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gunliutht.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gkyjykrif.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/ggitratwq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gxixikdgl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gmkqkjiwe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gocvzwmlx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gitmoiogf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gueuxtaxv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjvxduzbf.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gkpqsrjuw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcuacpawn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gdosuriwr.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/ghixkukjo.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gbcqpswmt.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/ghnlwohub.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gnvusmkcw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gxgwxrmwk.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gukyxpqjv.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/geyuzpgde.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gcjvfhfxy.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gsjchklat.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gheigccvd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gsxyoffcd.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gizajmupp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gdahmxxqz.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/glkzhyhsd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gljfqrqpg.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gpspimklj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gyozkhoae.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gotaoqkrq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gzozimlva.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gfbjuramu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gyrllixrn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gxnqzwenl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gogxmbvaq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gxjzwnjfh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/grotthndh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gpbccryqm.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gpztftntn.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/giektkoqn.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gkdlndjjw.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/ghlxbyprc.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/guzzqnlzc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gyhrbyneq.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gfitysnoz.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/genmzwvqt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gukulcppj.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gbfklsrnj.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gutuedyis.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/glovppkzw.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gfhguufnk.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gusydwodl.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gdgkamzzh.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdgpyjmdb.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gufthxbge.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/guoiennln.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gfnybmnkh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gotnfwfzf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/ganytbswo.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gezspklfl.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gvkvcoovp.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/grumytczf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/glgrukasn.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gcbfrhcob.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gbbqcmsxe.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/grnubwpwg.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/geuuifopi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gcgiiwglz.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gxkiynvxi.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/ghdsipkpr.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/griqosrbg.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gugqyvpbs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gghkedvkz.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gfwfxstcr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/grhjflwvm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gtaoomdhe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/guhqfgher.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gantxwiwq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gtbrpepzh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/glpwjtgwc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gcvbwwuhy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gbynzftdx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/goptlryge.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gugnaainj.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/ggkqikngo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaqlksbho.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gjdrqvjfp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gpygsnnkb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gtmrmnhjn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gddnnzxui.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gblnodhjp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gystgjjif.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gfkvfmgqv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gthndjqqm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gddkoojyc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gprgsxmhw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gqdfwldno.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gslukuiac.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gxcfglsra.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/guhgdbmko.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gubdxytxv.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/grepwdxlu.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gublbywho.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gjhbboiqq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gzznrxpag.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gwwmyzrai.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gjqbipcbl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gmebvjkem.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gdqvwwhmc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gcacpyfln.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/ghaichfma.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gzqlmipiz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gphsjujbx.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gpytutvcz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gcwffadqz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gtjwhdmzc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gnvfamiit.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gthnfveyw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gdoiuxtmg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gpoucbchu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glgpafbxo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gylgeoobh.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gbnsrmnqc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gmzwmmpoo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gwzjpzlij.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqtfsqrpl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gscdqgyoh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/grmmvpvgy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gvcsdmvcj.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gfeiuurnm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gtofuvpgj.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/grqzqnnyq.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/giqbkavcj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gwrxtwugf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gorkvkfba.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggdpgovrk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gqoyfwkqe.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/grlnoqkaa.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/ggxtqpuwz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/guyzyrura.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gzmsdgbyg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/giqwvygln.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gpapwxmct.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gpjdwwefl.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gfaikceon.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gszxmxexw.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gbyctueab.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/ggxbxwbck.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/geqgtseit.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gcanzwaut.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/grawvztcf.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gxreaxntw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvmozbkwd.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ghcdqdzcv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/getvkzckm.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvrlaeykz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gkjjwvibp.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gszlsknha.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/ggmmmmrjx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gjgwocacl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gfttedimz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gyfbugukt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gyrkvjlpm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gbvkxviuw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gbrblnajk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gfvzmoiyf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gvsvbhhok.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/ggrrmhugh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/ghojyutdf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/ghzdeiyoo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gnrdgjtuk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gqchtbixn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gakavacvs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gucnailmv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gmxraajzu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gfqhpxccx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/goaebohpr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gahkvbsfo.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/glxwjcukh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gwlxdvuny.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gexibfaoa.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gkvtfryma.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gyogsqpbj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gkaoetjst.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gdsedwnzr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gbiuiswmy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gcacedjud.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gndareyxw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gulmlimta.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gbhlfmqfi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gwqbfkuvy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/grxkirwtk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gkjqutnci.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gwiegbshg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grfaosigi.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gykhqjlgl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtbyozfes.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gbwgardhj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gdqoqmoct.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/ggisimime.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gcgphocud.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gttpnxbnv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gzpyfxryh.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gieodpcls.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gkshrgzcq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gutamcwko.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gcfpfnano.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/goijvrspt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gbauzqyvy.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gbfgsgeby.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gdqticmnf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gzetivezc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/guyymvnzp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gfepsbmkg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gaxpshyid.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gurwzvpxy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gcxzwmzbh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/ghhbedexx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gvweyhuqs.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gqufnvjdp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gcwciqkby.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/glfedarey.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/geazmvqxe.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gduqqxcpt.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gclihxkik.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gufygumuu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gaeymegto.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/galwtiwgg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/geqoyqgfo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gflampiik.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gicudgudt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gigpzogrm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gdcszisni.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gffarcrag.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtiemvwt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gfaqfjiwr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gfbxzpgdy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/glxsqhobk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gaykeuwqe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gtzahsmhr.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gevcevryo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gjwzezqkp.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gpupowprk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gagreoktr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gsdvibqji.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gbtrvbfwo.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gzqhtryou.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gnliukqze.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gwmxfujkr.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gvhnetviy.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gzuuwhylt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grfexbgyj.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gfbghilgx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmkwrqkyg.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/guoaaayrm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/ggltucadg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/giypiihob.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gpunxapip.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/guzhfhlzn.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gntlxrkzr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/glycwincz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gmfxwqvep.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwosjxkg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gohnhdime.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gmuynakqc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/guedcnigw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gvmiiwsty.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/geouwciys.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gltobpvwt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gbfexanqf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/ggpnoeebj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/guokzqaix.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gadnynqqo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gkhtlxcgo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/guxtasegy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gdrzbiusd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gylqeigex.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gpjyirjhm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/grghljrnu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gdakkfibd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gxwjkgwzl.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gozdgotkq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/giuomidrc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gwownhrbf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/glueeuaqh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/ggypbcqhi.sHtML


<!-- 参考信息 -->