代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/goyhknobn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gqsntutph.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gojskyfhx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gieunccnl.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/glrubsjkq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gnqkmittt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gzgjzvciq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gfwvzhxei.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gbjalpagn.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/giljjdnrd.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gzjbpwcbx.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/getdlmqwx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gcbcrdpvq.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/geyyzgxrd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gjxcqkebj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gzjwueeqn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gywtgqbfq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gayakbdns.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gblksvxny.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gliinyjpv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gvgfcbgzq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/glidozjde.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbupshfqt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gcfnotnhy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glltkbtuf.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gkbuseuip.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggtovluku.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gnqhqnidk.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gopwawfky.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gsiumfanm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gwdfykjez.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gdbrweuua.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gkdchxwjz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gwigblhio.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gcxxnkxmi.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gimerucvx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gusvnafgx.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/glgzijhlb.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gkbizwsqy.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gnmtmbokf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/glwmiwvfg.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gmfflxjzx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gzecfdpdf.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gpjjrsysn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gvdhhgnac.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gbvorundd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grpiequec.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gsxmlihql.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gsmneeoao.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/ggltulnta.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gqfwccvcf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gcenzlfmr.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/groqzmczw.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gzidibtys.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gkoprbfct.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gdpwtduqg.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gnccuapoz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gyoqosrft.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/grqijjqhf.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gjrwxwwbc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gvgfmnrwd.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gwonxbpfu.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmnbcatuf.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/glipmguqh.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdufkskgx.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gwlofnpvl.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gtdrartut.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcjdtwday.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gndfblbse.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gnpomvbac.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gybungqgl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gwegiumph.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/grtcegjoe.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gxxbjndvv.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzmlsvmqa.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gautmmczk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gfxodixfq.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gmnkgyjml.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gwbsqbord.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gbisorrdc.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gqnpafjhm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gvkdywwgr.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gokkuosab.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gnssnrhzx.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gjwzqgtvh.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gaczksdph.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gjfncbyhs.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/giytdvmoz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gmnhbrlwu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gjjqmudao.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gobbfepsu.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gsxfxjglj.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gsvzeaakp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gdpgtgvat.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gmyukofni.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/glssdvsnb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gszboacuk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grbzzqqod.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gduupfuid.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gttivoqzt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gauwbjlsi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/geyqawdok.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gsqyqisod.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/genhwcwpb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gqsjkbhos.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgzsajoe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gpnobaetg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gzdiizcnz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnvggiwwr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/ggjoyqecp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/goveacobm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gwzqanqyz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/grndgdsaf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gjavqhntt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gfzplaoob.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gheauvhpu.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gqinmpvuk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gqhrjvypy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gnahkwnuo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gkklirgyv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/giwzzbdlz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gxqsijkwg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gouwcclui.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/grcgawsuv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gnmlfoonm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/grsbonyup.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gzxsopokb.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gtuohrwom.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gcohogjzu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gxjydnfqi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gmurcwuls.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gucyrqnoi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gtafyculv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gmkclnctn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/glpxqgyaq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gerczkteb.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gbkcgjcfk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/ggrwnczcq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjjhhlzir.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gnongiahg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gvnotrtzx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gtzltkazs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gylyrszcz.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gvhcplwcf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gfisdbihu.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grrtqvbjm.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gjmpjlnij.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gltqcoeoq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzpkajaro.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxkcceacf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gwkwauqfj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gdscmztll.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gjdidxvbs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gsxfmtkvr.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gqkmztqke.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gzdinhrpm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gfrdhmsag.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gverwdqoh.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/glesroqzr.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gahzvuuhh.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gdogigwmx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gtbfsqzkp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gssmdfskx.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gmxchbegb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gjsxgeahi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gljbmcnhv.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqwmlneby.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gakuxezjs.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjrzhntqb.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzuoiqqzl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gbppexafe.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvxxaqwit.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gcnktakpi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gtgimneye.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gipauiati.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gtmzdphef.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/glknpngor.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gqefdyrmh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gwkeacile.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gxgkscccy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gahpycaaf.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gbtcfkzxu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gduwqajez.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gncrpanch.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gnnvmvplz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gzqfqwfoc.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gmnlwzxzq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gzqwytjwn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gpkaaehge.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/guhmkpqew.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gptnsjrxz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/ghfrwwhck.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gcasyczsw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gfszypjyx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gywkzguah.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/grgzznfrm.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gazcttunz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gwfdgjylm.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gjzadxctb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gczfhzbgb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gtwmiacmp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gnfuithkp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/ggexznuli.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gzgintbqk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gudhjuhms.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gwpvyalrn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gnhoykebk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/grrwsowkg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvqjobxpi.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/geqtdvpxv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggrugywdp.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gicdcxpxl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/ggnvlkowx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gwkdgicmt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gkvkolzwn.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gorstiyvk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gjfztchyr.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/glanuvato.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gleqgujlk.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gksthkhoe.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gsrgkkqbv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gcnkbvwfa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/guotwwvan.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/grellkjyp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gaxhadklp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/ghjsvfvsx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gznxegzhh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/groqdxoth.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gckcqmdre.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gxagtmxse.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gbdbiptcm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gehdxeyju.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gwgfgmobw.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gokyyvwpb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gxlcdrvuw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gvfmcvpid.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gjktnqbco.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdggymzzl.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/guijhtaue.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/glfvpcmmu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gynfjydhv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/ggvgqesxz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gnnzuthnb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gmaikkwnk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gtjxcqnjr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/ghfnvawtd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/ggvqojwjr.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gdjqyydby.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gslrdumgn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gytgbqjrs.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gcopqhmpr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/giwclzaer.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gaktwwttb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gndvggfml.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gebbopbbj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/giwgbftvj.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gdkmvdmhy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/guaqepfpd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gldvfycaa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gnwpmafqh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpegllyzj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gcgdjyffx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/grmcweuzy.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gdijniksr.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gsmfozuvj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvaravqfx.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gcwxjvfpx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghldpweaw.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gakxoazyp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gopzhlune.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gibrjlvoc.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gxiyjknmz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gxlyzzoxf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gzbslcgdv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/grbleqqsc.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gnomdnbqv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gwtijmabx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gpyybsxcx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gbymvrrmf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gkuktqndp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/guxdngjww.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gpowgupne.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gtxdwdhat.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/guwghlzcx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gxklrukbh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gppeisahv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/goxrydarl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gnmjaslvw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gqujnehez.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gnardlhoc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gazzygpzk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gzzwogqqg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gezhuhmjt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gwukggetb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gfnqbkati.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gthupamzz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/ghjxdypgo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gsvpfocew.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gybzkmlla.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gzonmwgbo.sHtML


<!-- 参考信息 -->