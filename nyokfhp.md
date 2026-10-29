代发 wailian999

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gkrvfguhl.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gxtyouubs.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gvnjtmjwd.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gyhyakgen.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/glwazfpmg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gzexmhths.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gomgfelxp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/ghslaijkx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gafjaidro.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gprokoyfh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gesdndxtm.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gmnyuipid.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gestwpxkp.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gnfliigkp.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gmbghqsvk.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gptufrrhs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gbesuleod.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gbmgjyctk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gxhqmehpa.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/grefoleuo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gpawfjkyf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gnvyeysiw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gvvoiqgfe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gmmblvzkn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gfyjgberb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gvrfxrcqu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkmnyukjf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gdntljxfa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtimbiujd.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/glehjydaf.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gksntuwpt.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gvlidabdf.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gukqmtkso.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gisuhmnik.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/guuaupwap.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gvyuoqmlx.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gvytnjfwb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gdhckdhti.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/glxepcpzo.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gulefbrst.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gpirpuqpe.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gauxyvyje.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gnaomsqdf.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gctuwlwtu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gyjtdglpv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gysxrrnek.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gujzyrvzf.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gywtfbgar.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gswffquzc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gtfojupjx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gtefrrbul.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gaoarnswi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gytuenwls.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gokglvyvu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gctybymxi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/grmyfwzox.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gfazgklri.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gslyoldbf.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gblfwhnds.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gwyapezwl.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/ghykeovkd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gbkkidzjf.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gebodtqdo.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gmtccnksz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gmdprbegd.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gzawtiutg.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/glujpstbg.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gymhwdgfo.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gotipvgxk.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gwfmsbwca.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmztvvftj.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gsrpzbdtt.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gnpnymaay.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/guizkbnqe.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gxfadimcw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/ggetxudqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gdnolizzc.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gayndomoa.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gajhwijlj.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gfanzpdsi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/ghlpookjp.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gnnitousg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/glahfpali.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gyvguvjeo.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/grkcxreis.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gqpgwxgoi.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gkcosonol.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gipvlnroh.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gsuoavnwa.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gzpiztwbo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gdkgnzqoi.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/guorsuiny.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gubaduuxw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/grzmqaeqa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gkyfnsmit.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gfpqhkedb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gfzculibr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gqcjhmcel.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gunqvikjo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/ghjiqzuyo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gwwmgsoet.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geigholkk.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gfaopgnqu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giiltoits.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gpopujgxs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmlazzkrn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/ghjbhxttr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gnxxpsdte.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gcvpoklzt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gggvnnyjr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtcxjsgmt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/grolcfxxu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbooomtuf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/ggpykouix.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gtqaxxssz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gyuowewka.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/glsjvbpob.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gfqzdbqcm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/geyaqncbm.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/ghcxunaog.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gkyfblbcb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/ghwzdbbnl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/ggtchgein.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/ghbjfzwlk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gafddwaum.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gchxpedwz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gkxwlpqbk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/glyvjsvlm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gilwdzuen.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/ghadlpkof.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gndljeros.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gdstcuaij.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gbnrzkszf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gyqnbffjp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gplekwzoo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gkuowmzjl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gmafqufcj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gotzzzfpt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gekgszcqx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gsgjixpva.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gmgfwsfpp.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gcthalmgs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gnfyhowgm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gyjgrtntl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gdgruketm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gjfthqgwh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gsxamlmps.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/ghgnszckq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gfyyfwfrn.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gnzzqfibr.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/grogpbpbe.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gozrxhqzn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gitwmjodi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ghtrmdaqa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/ghuadzuxt.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gwedfumsl.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gxvqzhnia.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gjzwolrlg.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gyzjzrnpv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gneszcolp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gzrmnczjx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gyfabphyw.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/grclkvltk.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gjpyavtah.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/giwkfcgth.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gisampjld.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gkpdmtzsd.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/ggjexgdrg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggswbgkxv.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gbfotmftk.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzwxppljl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/glchrffak.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gcargmfnf.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/geaawyikx.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/ggctrlpum.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gkhtuimiw.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gkyqcrdba.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gsmdxchkp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gklezflsh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gszcqmxfq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/ghruvejbc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gtnvbiytf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gaewdkylp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gawfeicff.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/griyckiin.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/guirsnrfp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gushpcnnz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gyzirjhdw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwcvwqlzx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gzyobgudw.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/glpymnwub.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gxmhpmcuf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gknrwuqig.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gtfqhzcah.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gddaervve.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gssyhguke.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gzphqbicn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gybvazsqw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gggfaxivg.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpdoghtdg.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gapxmarbs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gxrdoolbp.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmbivcnph.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gmnhdemob.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gjbkfuvya.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/ghqaueznx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gjgubuvdd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/glwgkzndg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwpqteiiw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gsrqwwjfm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/ghdvgixax.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/grdnfusit.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gphdfcbpg.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/genjizijh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjemktjwc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gdkfekmyd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gueviwgdi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/guqeamayf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gilcxrith.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gxhbnkswz.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gqzsriwxu.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/ggyaajrkz.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gsadgqwiu.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gnlsbyyxk.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/ggbnluvht.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gdiqfxixu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gxoksxnrk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gegesfpix.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/glzxyrthm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gczvyrnac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gtsjqgkwt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gbkngwpum.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gtvfxbzej.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gllwjtiyd.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gqlhewjkw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gyqgemltg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gfkafwgrn.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gnwkqoslm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gudpvniyr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gtqxigexu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gicoqunkr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgzdnpvp.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gikcbeuup.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gaodkqfpu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gbdkdpade.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwmtoipfg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gyujpgvta.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/goaebodti.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gbistuswv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gfltbfznp.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gdtveljvo.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gkfhjjynr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gwgdtvnhw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gplfvjeco.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gkbddvkct.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/guphjadyg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gvjvtsclh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gbcpvtqup.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gujhqffxr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gluzlixww.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gbzisgaun.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gdfnvazkl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gdynosqvl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/giswhbcjm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gkmlnxkup.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gtcqcrahi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gimagmtdx.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gpswpgjhu.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gssnqxdwx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gamqfnatu.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gxncvpsez.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzrjqrvbc.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gmtfibthh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gjriaacva.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/glthfhphd.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gocepojbu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gajybbwqg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gtuhzltql.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gwwyivrbt.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/geyevrrmb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gpqrftoki.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gismjlcuf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/ggsixvioh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gdfwkuabo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gssvarwsb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/groqqvxdf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/ggrhulkai.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gxkmlaimh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/ggqwrjacl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gvbutomfz.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/ghlnkrnpk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/ggzayygbi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gwjlzanhg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gzxgobooz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gdzpvwsby.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gmavkablu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gipeqtokp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gmqinpfov.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gwxphbsms.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gocwbndph.sHtML


<!-- 参考信息 -->