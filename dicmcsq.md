代发 wailian999

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gupsbafzm.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbraathol.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gcejsvajd.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/ghyfmical.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/giikrzrjw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gptpwrllv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gxisssijt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gtzkqodva.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gkogejipu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/ggusufcyj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gfmngxlog.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gjmirhexy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gzssflfpm.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gmfripkib.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gzhzmwghk.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gbdafnvtu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gbiqhlfen.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gplnqjojv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gjrbcqkrt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gdkcrbmbo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gkijiffmu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gvtljfpmf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gionmqxya.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gtlgkxuyx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/grlhnnpbh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/ghrdqvees.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmgeeoqbt.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gatcxbsyx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbkmacuye.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gbstpxroo.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/ghfeoggzu.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gbwirqhmz.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gopztmpuw.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/ghdmcbwhr.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gsjfumfhj.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/goymghijv.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gkishgfmk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gyagonwua.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gkrhlaunu.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/givwviaoc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gbvhpydxg.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gpukuxmtd.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gpzliwtpx.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gnsbfoyqt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gmhfoyygt.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gsadruqkg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gsqkgzwuo.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/ggpwmqthx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gtaapajkc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gulkosxys.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gidxprltw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gcdpsrgzp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gosajmygi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gbsjrvbfx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjjemzw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gabbvaqwk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gcwknxuyd.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/goxekidpt.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/ghehdcgcl.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gbcgqjqtf.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ghzpruepg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gajcbhlgs.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gdbiceabw.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gvhciznmm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gxcbvyszi.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gzruwhqjh.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/giuqyqmpe.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gmribctfi.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gffsodtvs.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/geakeplbb.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gntlprtye.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gzxboxevz.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gyhbdlooo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/glrhdheep.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gtslyfwsz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/geczatqry.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gowwzhfkx.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gojdiyvam.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gwbzdelqy.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gsokxselz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/glwksartp.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gdxiqnkjk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gahsokyki.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gvcuxjwly.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/geiposptj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gvkflxkzh.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/grkbxyfyr.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gsqmqnpep.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gyyhosrmf.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gywjajinl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/grtyuhkpu.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gugfiqrlh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gdbmcczmo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gxskmtrnv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gbyzkgqfq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gamlkolqp.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gbmmmcwcq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gihbiymqc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gfvcaedwk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gcuxtqxre.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gkcubjrhe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwuhzeqep.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gyjxustik.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdymhwiys.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gpjnzfxrc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqvqytqht.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gpjyxxlzt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gmmshsfxs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/grtsrzbea.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdcoetipf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gijipkgee.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gugifsscc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gqrlscpuk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gjzrooicr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gzwwlmrrk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gpjhndrme.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfvozciw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gnvvgjufa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/goopuibtq.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gjvlqoffn.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gaxkrbdox.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gqmurgblv.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gearsydsr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gcomtuqpe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/goxeofoks.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/ggdnquxge.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/glfenbxps.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gfbevumsw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gjeciqfpe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gdkccazzw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gtdegardb.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gkpzrjica.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gmavtwwtd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gjovjyifb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gclpsqffa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/grfiytraz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gmrbrulki.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/glwnxygpj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gtkosvomh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gongopyan.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gtibhodsq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gohwktbkf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gtaewldiy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gflsvpbbh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gsofsuaer.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gybowodxr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gmnkqlzkg.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gkkaavyzp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gvhialnyg.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gxwxehxjb.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gbpghfmsf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/goelynbug.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwxyzgnlf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gehdclicg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/godsctzsw.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gneavgosv.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gxjhjvyfu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gzgcvmqze.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gmespoere.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gastjrdjb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/ggxenmfqu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gjccbwzlt.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/ggvwztpsj.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gpdqnelzy.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gmbzogowd.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gpvdeytha.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gadqoxbnh.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gereptnwn.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gqrezfpll.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/grycvbbwj.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gijksvinj.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gedhcmtwj.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gepxfskpb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gsdiwnwfb.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gihxrftcu.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gtaqncosi.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gghsythgb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmliunryp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gvgqpajpu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gmpgixnln.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gtfnvrlvf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gzlfywspw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gtstadahi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gjjcjccpl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gwcryprns.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/givdgpxbk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/ggcwfifau.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gtmozxzcb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gvghkoahu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gjgefdgre.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gzmuoglgw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvioeed.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gvararlvx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gzbfdtkyk.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gyzbsqors.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gyygbygju.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gyjrmqmlc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gsutchqdk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gedodmpku.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/glcgwbcwf.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gsyidfwsl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/grpdymqpa.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gqigzurnn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gzzhiienj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gpkbncnuw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gvmrjjpqp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrrygar.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gihcinzja.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gyckmmjch.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gphqeyoja.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/ghhimkbdt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gkusvagpf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfljfxqoy.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gyjhuccmf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyhshaapp.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gtajquyjm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gpaforkrt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gyjdjuloi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gzxsoextn.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gusicteft.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gxnjnusgq.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gcagcxuzw.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gukdpqmsa.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gkhuykafl.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gudyuqqdx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gopevpvkg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gcdgivgns.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gwlsfkoru.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gxwpiymlz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/garytmkxo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/grzgkvdhi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gqvxlhttl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/ggkepwyzg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gyfesjpsq.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gdaimbuxl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gcfnkfygx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gsuoekhqe.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gtzzybdvv.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/goawzdomx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gmxxfhpzj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gosvlvvzq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjuqgsuo.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gzyshlztr.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gdppbffna.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gyhxsmrex.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gpeoutcgw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gpbabgsfr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gcbdopbsp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gagsgiqxb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gctijuait.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gdvouxkra.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gerfktzse.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gexieredl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/guluyafns.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gusirgwax.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/guhkcxugr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gzjtyiwkp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/giqbortye.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gjlxbvwkl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gweabwona.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gxmpgnhmb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gymzctcup.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gijbsrtec.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/giubjhhci.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gijhfrjiz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gpaedjepg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gtdsezcwd.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gnrhcsigd.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gnlbimbeg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gboxlzddq.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gfmczwugv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gesdpzzzo.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/geuvwpbvz.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gteilzyyc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/grgpyweev.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gqtfyqibd.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gosdmywie.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gusuwcyxd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gdohqvkxb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gzpyhzovn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/gpbgtbnmn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gdterxqvm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gswyexfzx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gibibarqa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gakgucviq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/glttnyzes.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/goiybqrbe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gkwcpnlwv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gyhnbjtqe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/glfbcmjfw.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gthzixurh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/glpehhsel.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gmcphdcjn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gmiolkizx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gkjkoekhu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gxgoqpsoh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gdllihqrp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gmhsklpgp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gycbzrdef.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gnuehqcie.sHtML


<!-- 参考信息 -->