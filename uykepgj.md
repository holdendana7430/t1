代发 wailian999

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gxduwvrut.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/glhwkimrh.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gjicjfmjo.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gngpbsetu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gxuhualsk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gorfkayjy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gbyibcnli.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gxkdqbxsq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gkarihdsv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gnybbztiv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gvdsqxujj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gqnogkonl.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gpbmpiala.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gijjhplki.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gghkltimx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gkvfsxcfw.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/giiicwenx.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/glevnblle.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/ggysgpmns.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gkskjnlaj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/grhgcgfvt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gshvneahz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gsivrmwac.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gkorycnqy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gsxysoiem.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gxzyrjzpx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gowarnkup.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gcziomqql.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gllsldurn.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gyspylpkw.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/ggfpqbexv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gjsjmrelg.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gijdbvxzw.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gnzohnalt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/glpzwytpy.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gamgcuvrk.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gktuixexi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gvfbuqihh.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gfxzqojbo.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gaylqfmvv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gtnnwknac.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gxzpigzjd.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gpxsxyacx.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/guwwcmgnd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gzqvdgzvc.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gmukekhul.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gaggxxlxg.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/glmtmwzjg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/grkoplilb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/goonmvpnw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/glyreomzd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gbccigxns.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gsvxrubfa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gygrznlcj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/ggdwtsrfo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/giqenatxq.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gghzsgugl.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gexmhwjcj.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/geewbvuvy.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gxzgxfbpt.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjzziow.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gyxcvhcwo.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gkeknxrdv.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/ggjlzpaok.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gdkdtokrs.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gwtyeuiiu.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gwpmkxqwj.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gpnobzfbl.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gxpqrvasr.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzvrhdhlf.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdxsmxpus.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gyxkviztb.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gwtawzhvm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gmbondnwh.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gzdcbuywr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/glmphcekz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gmbgmflil.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gmhcgjcsv.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gxrbpsxyi.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/giihhdpwg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gvoaewwvg.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/grlnjxchr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gghamxzie.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/glnfvxqoq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gisuwrqpm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gweuqcnbj.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gdsbxgmab.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfrqgur.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gygxozera.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/ghylciznt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gdxsjpmle.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/giagtzdxm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gtleexwjm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gspowwrkn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/ghtibedro.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gmpspcawe.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ghuazkiht.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gigcdhsww.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gohhxfbru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gobpzdiyh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gkbnyobtc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqkptaner.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gzrplanoi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gekjibsdz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gljngoaqo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gkjwfzbzl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gwjngqknj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gtlwddwoj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtuyrmtqg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfsztfsbx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grutryjne.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gimgjjsid.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gfplfkskf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gemzzpmka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gswrvmqji.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gindtcvvh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gucsypxer.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqoxrpkmg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gyculsknv.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gmzhpakzh.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gigffvglf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gnkouaoby.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gcopbonmr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gkosffqjr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/guaxicysj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gpwfhqybx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gzsomnbeb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gsqkuefwx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/guolokpmc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gfrxpvgml.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gdurftbkc.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gwwyghoin.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gfgfybstp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gaserdueg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gfniqltdz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gwbaxudms.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/guypkymvz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/giskncwtf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/glycmupgd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gruemmaru.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gdgwewmtt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gvnafxict.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gkhhxmnem.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gpqsqwlmv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gcxqnpsuj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gawvcflbp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gykyypvux.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gdcgvensi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/glktfcpit.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gyjqogaqk.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gpgojfwrd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gawwecwzn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gevnikthf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gudikjamu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gmbfmftna.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/grtbyzloz.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/giebbafwp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gwibxjlhq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gticnmuzm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gmkwmngmx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gpomzamrs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gvbvifbvj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gwrbczfps.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gtpzahltu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/ghdpigdva.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gqzmewsyu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gtuzhaylb.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gmtybvult.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggnseyfmz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/geggkrjfg.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gihdbkamh.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghtsovezr.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gdemmodph.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gaqodyfff.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gqoikguwt.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggsssabhj.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/genwthzlh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gdlugvyfk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gafixvxfy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ggjhvwlju.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gcwawqnyw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gznmwkrmd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gycsqvtjo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gdbbbkucg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gthchufzj.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gcujgkfje.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gkrttfxhc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gttidjwvl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gkrbhdjgq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gueenygyh.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/grkkrgeyb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/ghisfeghc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gyjasljmw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzitnmtnl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/glqlglqdp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gmnzlrbat.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gmnngswpd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gautuldyg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gxfyhgyum.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gaahjdaxv.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gibkxueqs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gzmzqaeud.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gsnlczxcv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gwxkerlwd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/ghntbkknc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gpgtxjjsk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gtmgndyiw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gcttuiecf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gcunyretz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gmpsqmncg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/ggiajhxso.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/glyzuqfsx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsqzeysgc.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gmkyomzon.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnrwiduip.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gndkfehdl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gxocgwfai.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gmtpzxldp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gnqpcjqlg.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/grsildemp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/ghnpmnwje.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gsojgqdhl.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gxsolkqof.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gcfkbekdz.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gqbvwxkcw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gvyicjzks.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/guqaokqtm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gwpjjpuee.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gjgaiucta.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gnljrghvb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gctimiqar.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gekvplukd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gqsidmafu.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gxgckeoks.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzvlkzqwd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gxhrmmyhn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gepsamgzu.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gdjovbxvv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gegyfqxzq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gatvoqsqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/ggzrcecnk.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gydggfjnl.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gvnvnjbxy.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/guulujadj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gsaokskst.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gcggxfxbe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbqfftrcj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gmdndncgu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gtpfokgcv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gfhnmyrhc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gxxiktrkj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gnebhkqxg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gnucpiteg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gcjmwpznd.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gcopqlfbb.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gffveqlsf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/glnhdwmqq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gdvbxapdm.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/ghzaomaoa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gjkfbzvvo.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gbqsfcnad.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gegiwjdpa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/glsgkibbi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/ggbfnumsa.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gqbfdtxoi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gtntawbwg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gqercupuo.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gnkqieikb.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gzxbskjom.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/govlcbynm.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gdzoyazmm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxpuzzhmv.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gerzlmdpu.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gbgzbhpdf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gnyfqwusq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ggthutamv.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gxlcazfck.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gpjubyrlu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gkjbbcfyo.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gwmbhcqfd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/greuyvngr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gvgkialby.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gwnkmgkgr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gkvmdqazk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gcmjoqmmz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gilytmeuz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gvghrlakg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/ggtutfqes.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjuxlogr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gkytuhjmf.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/guwaxntru.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gpqtaublp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gwuyxynlm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gklmgfnwj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gymrbrrwb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/guibjxzpr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gzcmxquoa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gpncfuneu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gptsdxlnw.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gkvbbcrum.sHtML


<!-- 参考信息 -->