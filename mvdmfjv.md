代发 wailian999

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gwwqvdekq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/giqitksih.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gcieigiue.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gniybtncw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gycliickl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gxhkbjexz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gytsjunuu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gdvsurleq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gvklufvdg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gbptlmmxy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/goubamaud.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gnejzgyfi.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gkkqhryst.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gmgvkputv.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gdzsfleku.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gskmdghwz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gdclylbvd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gjuqjkoor.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/ghhgwaqwj.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gpmdtzkfj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gbxtvhlvr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gmvlhykyv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gwpgdiyqz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gipnyqege.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gpnyknbfi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gywlgfxaw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gazehywfw.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gedqantnx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzjraameb.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gagyjjiew.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gnsmzicjb.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gkdwziqdd.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gobfoibjf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/ggakwidvb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/guxkdruuq.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gpeevhaoo.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gyzgjwknh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gfafmergi.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gnpzgkonr.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gywcsftjt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gkyaarrnf.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/glnycamsn.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gmqytdaxj.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmklkujfw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gegaqaymv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gcxyttiyz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gtzezsmco.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gmqdsxnsw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/ghsnqlfsa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gtfgylruj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gdyrtseyz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/guboojqpn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gddrxiuht.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gkqywiefv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/glgwvcihx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gwlwsekwx.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/grgktased.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gagtiqqsd.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gdeyuvvlu.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gkcpewxxm.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gkzmioqzm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gpshzvguj.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gsnidxuqv.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gfsstyuhc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gglnnexhq.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gaxjlimws.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/goedvswkz.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gyvmokqog.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gakxopsko.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxsaqnpev.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggdolxjdh.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gxegtylpe.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gtlfbqfpg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gojpxepge.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/giuupxnmn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/getsknjqu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gfknyagso.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gvxerxuqn.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gapaymvct.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gygugqxxz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/ghwmsslrv.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gqlwzaxqu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gkakxrjdd.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/guqxbrdov.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/glgcggkkk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gyhpshtfs.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gpighpjgz.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gloyxrzqk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gcbpgxvnj.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gxteorxvi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gpxlqfmik.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gvfrnvjkf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/ghewsldaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gkaflodro.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gytvacljn.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gqunkehrw.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gcifnarip.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gpddiqkgw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gzdoxgiaq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gyzdxbhqx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gxibsoyiz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gggvnmzsj.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gxkkyxnpw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grsxzlqxd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gglvpvbun.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gizrqpblg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gyvnngyld.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ggnivxjhy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gyytidrui.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gexzrwiai.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gyxvvrnxo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gkfohhmue.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gssfwjmnt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gqtslhwva.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gjxpaoodb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gkqkvrczg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gjpqrxszt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gkcaalcae.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gqfcytftl.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gxzrakjmn.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gthdsmplf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gyxifdbfk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gtrrbvlrx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/glurorspm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/ghmezdejp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gahkivrzk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gzuivnjin.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gqhkwxebz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/godonrvcw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/ghnkfdxna.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gkwcfemjj.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gdzezwinc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gmaczzqhf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gqlaywbth.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gmgnlfcbt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/grtzirqdi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ghtbxcbzd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gtxtiytcx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gpekoltvv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gjutpqatl.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gzpljdemp.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/giyisdwbm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/ghzuprhqz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/ghrpzxfti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gcyxmyvdk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gnpuunhoc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gtydfljft.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gtxxprvcr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gxaboljjp.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gipwyfyml.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gfujuxzao.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gullasmoh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gglcerxmu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ggwxlhrbi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/ggmjryxce.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gojqdfwvs.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gwfrlcqpc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ggwpcxenv.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gehkonbls.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gdfqeslcw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gvgpvatkh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gzjxivnie.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/giofhtaxl.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gydqcyfrq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gyskrbari.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gcpbszvhp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gyvssuhwb.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/guvcvtkyu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gykrzgykx.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gjrcwdiph.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gparekapx.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnjieyiho.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmymyvbuu.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gcbijvqez.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/ghsgkgycu.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gdteomkng.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gmgyalmqg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvstacpgo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gqspsdact.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gyomueahk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gqdakxngm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gqwdqtmmp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/ggoegfssw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gmwpcgoxy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/grnqyzslr.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gyusamdjn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gehsukqho.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gvacnnulo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gldfgvhwn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/galoioapx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gnetmmfyy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/giqrmcluc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gdleexype.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gejibdtgk.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/ghrnomqnl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gmvpmdtbq.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gevhrgqrp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gzappkdzs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gofblkbzn.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gytufsabc.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/grrwrjwdb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gsawktozn.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gxsbnejim.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gbpgpvsvx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gxhhyhshu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gpsxfujly.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gdnytizcw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gvdhkbzij.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gxabzfwbv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gdixbyxzf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gslkekcnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gnbweafbg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gevozirkf.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gqxcbpind.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpbyhyrhk.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gnnmvfuff.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gruedtzqt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gopndzwem.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gtgjjljmq.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gnynsbvqb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gqwdblwgb.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gzpqeaygo.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gpdumvisi.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gvkxsdrsd.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/guomtqtux.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gaxhfmpqo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gofcjmsco.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/glmbfcqxb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gzpxzyyvm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gelgdubdw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gpntrabqx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gfrmpecjy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gplbraiac.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gifphcerr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gxobtrtsv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gnxvfxujo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gawfzecdn.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gssugrtlf.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gtlvakhwn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gihsqxeiv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gsmxiofrx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/ghslcfmep.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gparkdszp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gmjbhvlno.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gajsuiqpz.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gvulcdqqy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gaxdtxdqk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gaphhjllz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gcfwkyjku.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/ghgwjjpdu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gjngpwjez.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/guakhlpfj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/grcktjgzd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gxhmeiufs.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gohwdlvui.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gbsnwieva.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gooulnjou.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gczrcuznj.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gxgpluhmu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gowxostlw.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gfhhfvynr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gtsxrocya.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gxuffunod.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gacmdsink.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gkdzoljgc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gmslroncz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gjebqhbmu.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/ghtzaanby.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/grqecrskj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbuiroaeu.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gwkzvilub.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gotpfwrzt.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gqzyjyxwk.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/ggyseigld.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gazdgvlcp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gmbphokqr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gmyipvqge.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gllsehlel.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gldijtogq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/goxssyyaz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/ghbuhibbe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gkvzodrxz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gzrngupdv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gxwkfzwlc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/geqebioap.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/guqpcgbjs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gxewxupwb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/guvryryfu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gmulxqyet.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gxgphjhau.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gcprjrirg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gfwwwxqfj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gqezspqkd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gjnhexaxh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gczshpwuk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gsqfjqorw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gkfqtfiec.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gtvwvyrpe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gboujkxug.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gafmlggmv.sHtML


<!-- 参考信息 -->