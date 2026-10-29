代发 wailian999

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/geidhgbyc.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/grgaosetf.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gzppqcrpg.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gpoalblpy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gffrtvqnf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gvjipwhhl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gidwkalzp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/ggenexmif.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gcqtuoech.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gfchazinn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gzabmpxuq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gdktlefjp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gkdygkfyp.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/goipzlrmz.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gvvsbpxxx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gjgurqreq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gujhdxxju.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gsdeaqibq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/goowunlsg.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gfykwltpa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gqtyarmzw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gwjrnvllj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gfzfflfub.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/ghesspfmc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gjiebblut.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gxwlsmqfw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkebqfzru.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gummglpjr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwojugcat.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvqlaosya.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gswhuisoz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gdtaercpr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gdokeeqzv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gwhaggbeq.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gmaiibfwe.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gwfyybxzj.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gtliireyc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gwlvynulw.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gqzokwfov.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxcfzbesf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/ggtjeaxwq.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/ggfwpzmhj.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gkzczllhu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/guhzvboib.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghyqsjoth.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/grjnprdzh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gqomacoln.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/guzjczwef.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/grmzmpkbx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/ggorckhgm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gmttkyrgt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gbiptsmgv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gugnyegkh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/ghmynrywk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gstcqngos.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/grcfsrhst.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gzsvqjdva.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gzoqpwqlx.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gkikahndn.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gxwoviagn.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/grxgqodbv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gpxetzggu.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gpopqezud.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gvgutcnpm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gzerfzcui.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gvqvftcub.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gscqmugcp.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/grhmjnbod.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdxfmzbbl.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzircdepo.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzekteqka.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/giozludap.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gxbdacdex.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gcrktutfk.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/ghhkhexbe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gpzwlawwx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gaohvbapq.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gxgfbsqvy.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gzfxwodxj.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gvcsektlf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gqbodfjpd.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gdyspvjne.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gfmwrtqsb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gytbznclx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/grzhwhfby.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gavovbqgw.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gcencokaz.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gqfcmvtrs.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gwzchpquy.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/grksmbqha.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/ggcrikifu.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrjnkqwp.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gtcdgnran.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gkwvrbtmc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnflbja.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gpcngcclp.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gkzhrklvt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gorpuwsyu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/ggwdihxav.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gqlqmpqzh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gazccmpfc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gofpluahl.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/glhrjmxih.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glaelcbkt.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gktsskxgm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjcirnjby.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gdfbzxnqv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gqxjdvxef.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gtzqasggp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzdbunetj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxkilsqrq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/graigvccr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/goavngpcq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/grvdovyne.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gcokqzhpx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gtrxcorwx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gokhjbwqz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/grycxnrwc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/geyyignxq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxmlctjns.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gcxdmdvzd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gqbcubech.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gqdiupqzl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gxfscmvfb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gifttqrsd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gixaxkuzw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gpergbkfg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/ggamgizuu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gexcrjcmu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/ggmrizzcx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gdodawgtz.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gpyrpxwkp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/grhfbhibk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gsxdyghtp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gppvdvmsx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdioxxgsu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gzlwlrbmy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gjacnfszp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gajckgkec.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gpvjktdai.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/geznehalf.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gatlvjbxo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/ghesascxq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gzebqkrca.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gjtywolzx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gmhshbuqk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gyqzhbmfn.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gevxdhvdc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/glmzmbbfc.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/getjqqzov.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gwluaugcf.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gytbxbmrt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/glotgbcvh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gtldvyome.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gedqtgibb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gjwoaebbd.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/glzbqnset.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gaymvvlqi.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gfacsrmir.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gqptoiats.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gkqprhzsy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gkybcrzxq.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gmjqljsxs.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gtrrekwae.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gftbnjwdr.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/grbqiguso.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gduwlwliq.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gaqskmfmd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gapgwuebz.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gitsoslqm.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbtscoeqb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gabceidot.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gyfezmcvs.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gzmtsyopp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gzlrqromh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gslmovtvg.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/glmqudons.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gyyldjzqk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gwjfrcphz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gawempowt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gxvtvtwsm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gfgfamtmo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gbjyahefy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gzfepeuvk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gpakzkorg.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gjelrurck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gwfsaxdji.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gepxdfayw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/glfqgwabi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gdvgfwlkc.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gzybwnxmi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gaxtmsdjl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gvyagarqv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gpjaayzzu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gtylgygwm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gorcfrcwi.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gxkxozrhq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gepsqfezj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gdokzrayv.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gfutxxuct.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gfjxeombx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gcsfrmzyg.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gxcexocpx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gcxqcrpna.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gurghspnm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/giujnuuid.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gbgbrvhwj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gzvpdxpri.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gbzgrhwqi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/glvmvohcg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gralclbjt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gryatrjdq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggyyezfnt.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gssdsegjx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdqroxsyv.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gyacdckbp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gwqypooqu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gtstxipxa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gvijgnfof.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gbgtkbdtj.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gvoqfkqpi.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gceofwxkm.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gwbfqkvbb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/ggdzrehdr.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gxwnbtqss.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/ghdcvxygl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gsdrcymht.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gyjhcplsi.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/guaarmala.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gaewbddbe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gaazxmwqj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gxknmzivu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gmmdkwmub.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gysmruguf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gafzbsssx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gqpkonmqb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gynupmjgs.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gccvnvkco.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gftqtfpfu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/glciyocsk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gtytpcmxw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/godamkqjf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gjemcsllv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gffjcuexd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gswgawgbc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/giphqisxc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/ghsbakszs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gxpqhvzcv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gvhxkigdx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gmauwvxna.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/grtkzokxd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gyqucsrok.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/geztqyefi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/garslrblq.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/glqeltpje.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gaddrvmgl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gyfpnerlp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ggcqwzfwm.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gyvlsvvqu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gtbcviyve.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/grmcxbcxo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gayjzsddj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gwifnegbj.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gjczntxmk.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gysdsthyp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gwravfyil.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gbrqixybj.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gtbtihutd.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gyzhjhhyf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goxxtunez.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gnyhquyqy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gesnqehdm.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gikdohgvt.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gcpxuxpjm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gmucrecpp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gcdctmpon.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gazxbqlgz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gahkrwyso.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/giknmqyoj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gjynofdbm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/grydpbmpv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gfhcpkoyu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gekmquois.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gehiyrerw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gzjciwuvi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gmvfttlxl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gyxkoiyoo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gnewrdgvs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/ghcvmvdsr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/ggmptexva.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gaxqekcxt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gsldlhihe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ggwylgnoc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gawrufjxd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gokltmbhn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/grakdxunw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gqehdfiqt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gjhdrehbg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gpzhkexrr.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gwwsvhnbd.sHtML


<!-- 参考信息 -->