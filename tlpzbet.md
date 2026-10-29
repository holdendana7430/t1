代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gfzqmzquy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/guylrllvd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gtjkmnokv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gnuozebml.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gfsvwtbeu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gqczyqjic.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/glkqismba.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/goweftgxb.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gaohzeifp.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/giamqaqad.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gaqlxrroq.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gjptolqxz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/glbwmnszi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gdqitpbar.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gcjexuhgk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gsuzofrhe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gttogksmm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwztmcrqx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gzwnjtrrq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gqlayhfje.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gkwmhfmij.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gdnblbccr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gejippujg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gjslccizs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gszzgirni.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gbnrabmqb.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gtuhphekh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gkfhbnsmj.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gkxqczpqs.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gfwotsxyx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gignvcshd.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggnsasiyz.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gjuldaraq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gjtmlzsem.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gkvkbrspz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/goymljock.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/glutoossc.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/ggqwvesht.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gjrlgzpbj.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gdpvlfwym.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gndmjpcse.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gqtmfkbbr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gmeyfktny.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gcpqxpkyn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gjutarokr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gtokzuzpd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gsqwmpcap.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gunilbhul.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gzbslrkhe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gztwyuokp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gqyraltsg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gwjkgbkqy.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gxnrpxozt.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gjcsclyvr.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gfvphphqo.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gcugoksql.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbivuguow.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gfzqmflev.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gknixbsmr.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gvebbyizf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gsomgoxrm.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gleemnpiq.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gujymietk.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gkbzotqrm.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghhmlzivh.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gblulfpdn.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdryhysik.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gwlcucydc.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gldzmadha.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gayuvmhho.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gvdmzjmsj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gfawjleih.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gwpnmlaym.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/glhvcfbmo.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gahfnbcuz.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gpxfzolwn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gzoxfuegi.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/georvnvyg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gavysqxii.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gutwmyflp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gmhfgfnok.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gkgjzgfpf.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gqpomsrco.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gpsvzggnc.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gexwgrjcp.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gjkgloiuk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gmispggiu.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gotunusys.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/geojnstbg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gfrjtcuaj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/grcpyskmb.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/grgnqimet.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gisjmkxcz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/guroatmws.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gcacautfm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gbpkqzllm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gsugzvxbs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghvwtdjkw.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gzpjbmvdt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtiepmfxp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gzvwxdoho.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkimmzyxu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gysbjuuik.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gltrtzfrs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gtdvbwsyi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqihiyylw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfdxkoglw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvkqdpfi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnjjrckoe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gsorkwxpf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gmkcamzab.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/ggcqxzrxw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gjpdnwxto.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gvwdapuij.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gbddnshrr.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gqkxjtckm.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gaotyqfrx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gfmugpvgr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/ghbtuugtm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gabsjjhvi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/grfrhgdck.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/ghlrijzbn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gbjdoyjam.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gkhctveqh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gkecbodlq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gblgdebjh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gfzzvsbju.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gsgissfoh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gyvmbntjx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gqoxjusgw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghxehqudv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ghuimtrff.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/grkcpcmsm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gvqvsnzmu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gyqevxbbc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gambysxww.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gpqrgkvgm.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gkgdzxlbh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gkxeiwbhp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gtxqikcjw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gvrqlyrgk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gerubygmx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/giznqvkfb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gantccqvg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gqbsszkzi.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gheiulwnk.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/glhfygqsk.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gogxkpbzi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gixvhjksh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/goienzsix.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/ghwzwwagg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gwdkjzjto.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gynliozth.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gckgemulw.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gbevuhhhi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gsucevlsx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/ggnuddfom.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gsnidoioh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gfyazoocu.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gyrnyhslm.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gstoztkga.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gttvpsgny.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/glxvgzoem.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/girstjdhy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gysxuxyoc.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gdhmuxidz.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfsagrhoe.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/guneolcje.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/grnmtafys.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gqpichzbq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gugcxvgub.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghqylupzd.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gerxezoyy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gwmljderb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjlyyyrzc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gkeuzigtn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gsbqwlnyw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gkxtocssh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gsocmxvno.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/ghgxtguqo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gqeysakmk.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gjuceyjwc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gvhymzstd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gmegnykjx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gugvjjsih.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmqdcafs.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gsipcxosn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gehmuwvdw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gjjignmgg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gwixpfmdf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gkrcvgrbt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gbxzawxhv.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/giloijznm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/guicfasfo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gyvtmzkze.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gvvzussuc.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gxdofwwmc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/glfdlpvxc.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gzwzdrmxu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gmrdppbpt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gghdsoiuh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gsaamagwp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ghpaupohx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/garivsgic.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gmikpldxu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gohznszma.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/goglokwgj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbwxinprt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdlxrxrup.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gxigkfevx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsvqducnf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gugwumxef.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gqchxjgnp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gfgstenjj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gznxhmcfh.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gxqwzhwbv.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gmrsmxbkn.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/ganyzmqtg.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gettilnal.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gchqdmdff.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gpkggsito.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gbohmqnle.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gifhuskvj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gwwooofjb.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/ghdhmckfl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gffvzadsn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gifialgwk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gotcxueae.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gfedhwfzh.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/ggvmjkcpq.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gjmlirpnn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gzzsqpgxx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gaiubltpd.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gkvhyunmh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gwcudxkfn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gsveiwnqb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gfbpljzpo.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gotprnefx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gnanayqbn.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/grdxxdcbx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gvcjftbno.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gwlysxjbr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gwlynrhkw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gwahnsjth.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/guzdxqlzo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gajjwzlkc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/grpyvwgsx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gnpolcbsp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gkfrjdgcw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gmsgkiwhd.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gkgdahkez.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gjkrmyblr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/ghdzihzni.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gkmlgsvgl.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gfxbhqmtv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gowqyqype.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gqtagqlcx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/guocbeaqe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gqderapot.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/grwsqhuiw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gxhrydigx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/geqopqxxe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gkyflfhza.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gmcsypnrh.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gmwnmxqdz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghvbpgvjy.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/geyqmdnev.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grfpbznio.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gtfhlntjp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gmrsgxoul.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gvswrwxxb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ggbziwrpw.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gthljjwmd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/grkmbtyhz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gxhedvwwq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gfkgmgiaf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gskwueksc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gyqcfmhdw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gaztsjrmn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gcnegypkn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gfhwkuagt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/ghysyenfz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gwqfwsqgb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gdzxqypyk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gszzwuwvj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gtqveosja.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gxmysxekr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/ghihtopav.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gwjeqbwrk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gbldmvbiz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gpotfeytt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gyusrsdaz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/ggevhnetd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gspodmfnv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gjjaevgqd.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gjdplfsxs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/grnusajix.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gluhftqlz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gqoxgbykm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/glbzohufs.sHtML


<!-- 参考信息 -->