代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/glctemlec.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gdzpktfdn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gteutlbio.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gjivpsagc.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqedstr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gdztxdysg.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gbctmfuir.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/glxukdwfb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gjiznilwp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/geylvvrad.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gdazajfqm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gylbdsgqb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/guhzsdqlk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gahrmvhdz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gaoldzbhi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gqhrdkawx.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gbpcduhvy.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gaeqzxeqa.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gjtstihrs.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gopnuxemx.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gaalqwwfq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/goianouzj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gliopzuhj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gretjphft.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ggffzjwgf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gapafxtgk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gxnyqkcuc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gohkzatlf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gmnmjtpgo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/ggubbwzgw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvldoawlt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gytkcniyy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzrzpqnum.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gdzcsupjo.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gznimuvfy.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gdsusospe.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/goqzikjgc.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/ggskbbmyd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gklccueyq.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gpnhkyswb.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gemsxbphh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gankbdxms.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/glqclohts.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gnabhvrir.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gbujytxoo.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gersatbtm.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gnmadsfio.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gtkgfizmr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/grpucsmsz.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gourtjozn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gdktznhae.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gbuwgqldy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/geiliyymn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gvdyvsalj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gstaccqnx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/glybvkmgk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gycvkbdgk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gzhprhunx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gbqknpcxn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gfdparfqw.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gciyvfimd.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gxoviqwhh.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gpjgaands.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gntyvutqp.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gnjjfwcfk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/glaeorziz.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gwdwwnerc.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gkzxvsemc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gohhvorjo.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gbcdmcdyt.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwbuqungx.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/galmoweuy.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gosohitqk.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glcdeufua.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqvjnydkv.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gjerjsjau.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/ggqtbryvm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gqwnegcdx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gfazretaw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gvvcvrpxz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/ggdruyeqg.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gxclavhoc.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gwzlxuhol.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gjxkgllzj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gpqdklaqg.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gltbmvgit.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gulpbrkuk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/ggxcfkttt.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gplnadequ.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gchrakdzs.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/govxlnccd.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/grmxtvkmx.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gkhgnhuek.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gbtfnpatn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gtlfuvace.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gyvqadlzo.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gdggbbkkm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ghlzfdufy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/glvauhykw.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gtgyubjpi.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gkvgtazjj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gokdefkze.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gztbigcwc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkgjiyx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gcimazkrz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gysxncxdb.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gyacanygl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gstsfsxwv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gkkxppwug.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gejaraxoj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/grvuejbyg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/ghcuaskbi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gijgfigsu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gxtujellr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmnmyknt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gwdejqeny.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwdgeptzv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gwwswblka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gvwizmwfs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/greqbewcj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ghhnkekox.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/getsrgvpd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gvehkcazf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gxosyjwxm.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gfcajjugu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gdtsqtuji.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gsesccico.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gzdlgngxo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gpuxosljt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/grkazzalf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gncxvqdzl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gcwehfxqq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gnvbatpft.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/ghojllfgz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gddyutkfu.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gxgqkbyhb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gjqesauwo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/ghsjnnjrq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/goodpxjxz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/ghgdmspzc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gbjcliezj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gusksllia.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gifjllsnd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gsqlvftzm.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gevqhtbhh.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gfklmtirq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gwfeyeswd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/glaalfqli.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjxcjfwku.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gyfmecedr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gshklwmij.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gfpzkadtm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gpdarbmgq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gulfoontq.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gdtfpmwwj.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdslkjnkb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/giueercdg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gedesjntx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gnvqwuiru.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/goxltgslh.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gsrthztmy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gcdmaruyv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gtxcfjhxf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/glphozvbl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gxggzvxac.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/ggksrwsvf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gwqysvrpd.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gxjvwasvi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/ghgqgfbsc.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gyaegzyyr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gdwgsmsgy.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gsqelbfak.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfdxfajmy.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/geaxlyspn.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtitpfidh.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gudjkjspj.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqmsqvvtk.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/goifgruql.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gnmkrnvwv.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gewcbsiey.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ghebmypvs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbidebkuc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gbznkaojv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/goaugfueg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gotwhggvv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gssekzhgw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/ghexrcesx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwmojwbis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gmvplybho.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gqwpjrutk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gralcvaic.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gqxgqmiqa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gjonkxgfp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/grvrkgmcp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/ggzcjfwya.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gzvqsznih.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gfdtiaagl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gfaduynop.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gccbltwmk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/guznyrzsz.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/geoyxmumh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gvdyodbdg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gopardlfb.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gmggkfbrc.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gdhzjchfh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gtpaztigy.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gynxpsbnp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gxzvhyhjf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/guuolvxnm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/glvhkmprb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gmqtlknje.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gjusapwvj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gxhmithii.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/galkvudxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gaqdiizoy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/ggztxdxxx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsqexdrca.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/geossemam.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyzcyhota.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/ghsjyhgbh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gvidsxfia.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkqvrsg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/goabsciav.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/givsukdfe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/guxxpnens.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/ggkncchmj.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/glpjkwegg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gqiuwzsjh.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gdbpxvvwo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwuwwgihh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/goilqorle.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gjbbfgpkz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gghszpquy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gogtcoqxa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gdyzlorkz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gjkbxevnq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/grotbeubo.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/glmlsmikd.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gkupvsqvy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/goxkjkwpm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/ghayuuazc.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gfhqttgoh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/grmtnfuns.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/goxjjiyxe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gtgpjizel.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gybzzoavo.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gcjwahzyn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/giwvgzjmp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gxxlyhbev.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/ggftqjkas.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gxctrwoia.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gklpnzotk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gfphtgggv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gehxbjxwp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/grsdtutoz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gugrifaym.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/grigzfyfi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gpuhwsoxy.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gprekieax.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gfzgbmuay.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gumxwctxz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/ggqmtwgas.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/grdofzfmp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gcuwyxnll.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gewsbckhc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gutrbwitz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gaoskspsg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gnbayeabb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gdafmfaou.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gchikveyx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gjyqnhzpc.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gelwkrlqo.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/goyamoowh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwrgcvzrg.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/glzlznnat.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gocakxbgr.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxcgkho.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gpvuystqw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gqpdfekww.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gggnvbweu.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gfwtgxukq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/geuirkemm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gourzfhbr.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gpmmxrwzh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/glzcsqtks.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/golxnwlpt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gutltrdur.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfeyyswwl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/ggrgjwxrp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gtuukkozl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhmnbrc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gplbmgfbi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gfvqxtuxc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gnfddpbee.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gvnfgsgpm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gtaqpyivx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gubvqthdv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gtahakjdd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/girksvcky.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/grninklfl.sHtML


<!-- 参考信息 -->