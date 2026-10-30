代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/golgpuene.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gwjerroxe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gnqfvcpfm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gjyhtdhum.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gsrfbmbuo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gyngadrdo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gumhafpco.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gburxutan.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gemfeptxq.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gshjywgxg.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gtyliqrkm.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gaeqsvqjw.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gfjcdhict.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/ggndppzfx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gdtjrlqaz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/goypbdtbi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/glnakncjr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gmmjjnxht.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gxawqiada.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gwvvtjksi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/groqxxwbc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gvnztlztf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfabhqfev.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gpyqolprh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkgintyse.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/ghxmyacnx.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gucwqrxbr.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gfxkmaxqm.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gphjfpfro.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/glxxjzkhz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gdnkmwipa.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gjooulzty.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gspdoypyw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gvqgrdsqt.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/grdegzpqp.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gfkxbvmom.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gpmkdmsun.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gnesuqbsa.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gwdegumsg.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gsmgrgynu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/goesvpbze.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gocxbvhay.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gmupxvboz.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gkunmxpeq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gxkbruktu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/ggvtfmupy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/geznxzpxp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gfswrknbf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/ghtpzzpva.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/goovumgfo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gzuwefsaq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gtpermydx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gpkdfiyyz.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/ghlqlijds.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gufiaclij.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gqhjadstc.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gokbyttgn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gbirwxqvv.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdojlbjqz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gioghyqzf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gloisbtnf.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/ghmkawtwu.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gbsplfvup.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gpdvalqog.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/grghhgpaw.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkwupiliz.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghvytyais.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gsvudzwvs.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gdjrrlsbb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gdngwhckn.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gppfaxoff.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/giisljhlk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/guknhbhpc.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gftgsqcqe.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gacdtrokb.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gtbqlrgrc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/ghkjpmlgg.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gatdthlyt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gdnhgtcst.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gdekgfmky.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gjvuyerxl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gotypplha.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/ghmpkolaj.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gnsfpksjs.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gvgzdvrfn.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/giyspwrol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/ggohvcmez.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gzugxpjom.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gwsglhvjv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gsxkhqmqp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gbigqkbfq.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gylkgnyhk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gkgdsmjgu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gzesdbcpm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gjldtwosd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gixliffjg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gzqfmfodg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwzrtuwop.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gnekbnrnp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwvvqshsg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gzhmprsjr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbqlvrpij.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gmnreqhff.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gvdivwthk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gdjwvwfbq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtmelxldi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/guzdefxos.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gqeiedaxt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkaofxqwk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gdasbrovo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/ghnecvjga.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/guchaipqn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gnefwmtzq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gozdkugcr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gjwqwfhtp.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqegyfubq.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gbgjpkchs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gegwvntes.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gusfcufrk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gcfqgxyjd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gjyljssta.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gvdekfmap.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/goblrrsda.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrjrznx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/glvwtjfly.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gxhwrrnrc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gmjbvfwxa.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gxmmgzuex.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/ggsnmgypc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gkgeumlwo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gomkyqbyg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/grspjhuig.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gfeaqzgoz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gqkxghool.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glvfytxhz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/glbdltgpo.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/ggltlujst.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gzsqevimy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/geyiwrafb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gvtcdevmx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gdpfajyfz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gpopslisv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gsogrqrba.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gsedwabpg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gzltbscxg.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gyilivaph.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gcorzgagx.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/guggbyikf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gukjssyco.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gznhnapdg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gutjljxdu.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gljdznkwv.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gntirejum.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/glpzfxkco.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gfrcchpdm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gjzruyxtx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gnfnrgygt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gabhwvbtt.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gqknjcvwn.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/ganwcrjly.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gnmpgfqyx.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gvkzoulaj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gwtdugtwf.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gmekchlsc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gzrpkjzaw.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/ghcdbbnfd.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbpyyylpn.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbpfnigum.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdwinarde.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gthbqkybe.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/ghxrjaigh.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gjhwdddzk.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/ggybumccq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzgedsgxk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gmznpestb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gfyrgecct.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gluyuwzgs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/ghjuijnov.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/goauracaw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/grhsdffdh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gmcbmzmsh.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gynkdibsy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gdugbkmpy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gttwwgidg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/ghqubssdg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/ggcqxgjwc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/ghhpmxdri.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gsxepiaqi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/glrvnftha.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gpxxklqpe.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gigrzomhj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gvvgsohtz.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gncanahgs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gwllcqhfh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gdfpkxzbw.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gqitunhok.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gtngakhmw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gnyzhuwbc.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gulamrhtf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gxicqhkdk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gkulrrlfd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gwvbpkxwm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gvztvrtfc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gwgvtqhxr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gjjqidmfr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gpmbzrzgo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gfcuzbpiz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gtlfwnemu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzrtngtgl.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gnreicyuc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gltkleqcu.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/garvcdcry.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gdgfuqpnm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gllkkypjv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gozxsumzb.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/ghzikvnas.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gctxgijbt.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/griaxnein.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gtyfpueoj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gambndrjn.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gdaoysvcj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gjffuctnn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gvjkwrafs.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gzxyaoawt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ghirkwlpq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gdtvkwotx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/guqurhzwn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gmjcqyhuw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gwazhetdr.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gaftaxjqi.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/glxmiupnj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gzlkhvmbc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/ghpzqmrcu.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gddaabymx.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gzackcpfi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gctrbotmg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gdlytelmv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gzhyxwlal.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gyecimzdp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gepfcwlyy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gccjuofyk.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gvuxsgjjs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gjzvwkmfu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gczvjgfas.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gkjkvmyly.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/ggdmrvvxc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/ghbqtxyzg.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gukrisusi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gdfbukvjp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gynztvsoh.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gqqfkehui.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/geohckmxd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gejnkpnzo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/ggitpbcyl.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gdwhupgxn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gxpnyxdps.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gblpfgivy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gqqzrmtsm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gpcvecjan.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gqfthlgja.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/galgsohhk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gimzxmiks.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gebyswrqr.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/grgsbbgpy.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gkoewfhdv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpsqfzsgu.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gaykfcbzl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqdjgbifp.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gpwlooorw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gtgwcdycu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gfvmvyoby.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gszkukzgg.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/grwejjjmo.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gbccqhzbm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gjjwtszzl.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gzkhxfanp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gfsiadfok.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gpehmgltr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/goaamnsel.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gzczsitgj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gtiqwzqnk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gosglhpzf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/ghogusocd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gjznrpadc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzcqarirm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gyaifbsfb.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtzyddnlo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gjwjonyww.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/giqoxqwcw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gkmnemphy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gwtpvzbpx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gztuogtqy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gkkecnpep.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gtubbncqj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/grtipmjrf.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gqhwegchx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gcetdpyqz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gupmmghft.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gozwsxkoo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gzfcgnwcy.sHtML


<!-- 参考信息 -->