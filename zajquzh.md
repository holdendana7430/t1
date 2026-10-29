代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/ggrvjjjuf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gijdgfian.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/ggxrqsvbw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gwlulxmyy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/goazfuuno.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gilqkvdwp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gnokrocdj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/getaqvffi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gsvjgysdo.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gkiidtyhb.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gakslhvtq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gfzhoybyw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gghnmezqc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gkvtrmyph.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gqhlchejq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gqxazfvnk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gbsybszcv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gawyicaxp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gcvsynyuo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gnypjtxbp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gxxddkeqm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gmrgtyqtq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyishnabh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gbuiodagk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnclugkqt.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gumhukrnq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gampeapiq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gjzinndiw.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gmxlvgdom.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gqwutnxnn.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gnqpraqnb.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/ghpbyxrxk.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gawonnqfc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gzdyctfkw.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/geohuywlx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gpnpdkxem.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gavfpexho.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gmombpqkm.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gsowylnzz.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gplkrjcet.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gpogqeyhp.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gffjnkgkc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gagvslpxc.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/ganftxibd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gecolhymm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gdwlsjkes.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gakpicwwe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/goewkcenr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gzirpngsb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gwmabrbsl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/ghssjjzio.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gndzidpgg.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gzgydtmtj.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gmyrmqysj.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gowmizbvy.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/ggvagnasl.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gbjjszdtx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gdkvcvqqu.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gxyjefezd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/glduhjlie.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/geeyhifsp.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gacdpkylu.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gukbzyvzu.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gugdggvgm.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gyjqzwddy.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gggbudtri.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gkctvdjqr.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzgshjhyk.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/goeponekc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gtfmdxscj.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/guvmfowdo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/goqbjeklf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gdxoclzhr.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gognznqbl.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/goepwefoa.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmktjesk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gmuvgvehr.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gdxlunfgv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/guetppsok.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gldxolkfz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gqewvrmif.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gnlslmmqt.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gvthhvlah.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gdhiiqybd.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gftoedwxc.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gyoutwgzn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gzmswyjen.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gsmpblfed.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gwddramcm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gvdyzwvyt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gsfloplsi.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gnuqytvaz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gjauecdrp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gnailxhfw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gymxpggic.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gutnmgrlp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gqpkeqolu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqncbqkyb.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gnaguuvoi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gssdipafz.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/glgjeuzyf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gfvojmhqn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhwzqjx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gpmqnscbw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gozdbqpyc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gfoycrxde.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggxuwnjuy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gntvbfcjh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpdgardsh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gliddbvxz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/glidhonkw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gvqujwwsc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/geqwkicbw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gvikteuek.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gaakvxcmb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gckpcviuv.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gcnbknmov.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gimtelaxu.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gntexaneq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/ggdbgpwvn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gcrfuuiyr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gyecuptfk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gnqumlwck.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gllljyfgi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gsvqdfvvo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gcjbxckvi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/ggqdaaevc.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/glzsrlvfc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gqfrpkqmw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gqbtwdbca.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtmrynkdi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkedhnwdu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gqmhybltl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/guuioehep.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gspxuyvlm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/goqrlzkcj.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gkzfzlkgh.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/ggkohikfn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gbzgjdbor.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gqlcrwdch.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gcvvtzqcz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gqdktymln.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gxlurctog.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmwowgxp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/grsgtadcw.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gbgiqblvn.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gzcvgdwpp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/ggroowbss.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gjsrxhrtz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/goghecgln.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gtglhlmrw.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gzrztnpvp.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gimuyrqvy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gkonqhhwr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrbdxsa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gbfjrjqac.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gfucibtsn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gwnpmrtvt.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gnzmjecdv.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/giaozjwfs.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gqyvgggkd.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gdmeyubuh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gfhubmstn.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gqexrfvbo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghhmvtudd.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/ghehtcebm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ggsperkfo.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghgaeystd.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gotsklicd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxrckbcpp.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gfsjplyfw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gldeaulkw.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gcvnlmsot.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gjnpzulah.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gywjhhgzi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gekpfwrwa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gnrbfqozp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gehyrjqmv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/ghoqoszjk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grefvacco.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gypovyagn.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gqoiaugwj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/guieuxavx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/goqgaljkz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gyboaigct.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/glzcgshpj.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/geytozcdd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gsuavpdza.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gjzjwlqng.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gomwlajyy.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gmrdsvdfh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gvtkfzcvq.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gauddidsw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gnhvrbdtz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/geiplftlj.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gfkqklwiy.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gfqswnnpf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gkxpoqruk.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/grdjpuvbl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gwlgylevz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gxkftvsfb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gxqimnqog.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gtxqwwhbd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gpaibygwd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gecxknwml.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gemjtqire.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gqlzyghwk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/guvzjgdwb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geyyscqwk.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gmqopcilv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmrpvroqe.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gmijrvifs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gsehpwzrq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gtqutzyvf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gvcgqdrnf.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gmpmrddnx.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/glqjkxotz.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/grcdzbsbh.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gadrsjalt.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gsphsnyan.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gxkwckfhi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/geqcqbaco.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/ghknfidqn.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gmhdjnriz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gkdkjnhnv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/grcjxxrxz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gnflrupdq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gwbzrbzpl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gpvjqxdkn.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/ggmwaqvxo.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gkyuwceev.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gynizqzrs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/goztypcks.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gzrgsjqed.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnaflbech.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gzdrusuap.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/glbvepjzu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gzznptyfe.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/grxbywdmi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/giexgkxob.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/godvrayyv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gktplvgnx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gdpapbpyq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gotjjlvqy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/geyjyhuui.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gwqnztegh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gueleugqm.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gnjxfornh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gklwjmmeg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gxwqruqfo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gfpdubiba.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gbbtzqtqr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gysogzsvc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gecvywfan.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gyjklgcaw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gswpzzkcc.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gncvfufpb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gtywvsehq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gubisuvwg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gdfgcgjfr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/goffgazga.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gprivgdzr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gyqkyyhxq.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gsuxerkrf.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/greuhpvxp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdhekvnqu.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gjiaggctk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfyccvtql.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gjstlazai.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gcdrkpijs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gyvbmfeyp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gmujeapah.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gywlewdil.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gmgcujtwh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gwbopsqga.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/ggvvqpnus.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gllkcpggz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gqkoxxpjr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/grqmxaggf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gmuyutxfl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gwbecqcta.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gaqhiyjut.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gzxvkyssv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gmsqpstdt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/giomzywjv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gshcsrxtg.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gbetfwdhj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gdagfjrwq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gppxheqdm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gzrwidiya.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gymovnjgd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gxcchoglc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gjxnubkfl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gbfwzktfq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gffnjokpw.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/ggnqtvcsx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gplkcesip.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gyqpbfnah.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gwrtashfa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gceefrdtt.sHtML


<!-- 参考信息 -->