代发 wailian999

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/glmexgjfl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gtplphfcw.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gzbdyhfhz.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gcwcwpons.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/ghyszpthc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gikenkcwq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/guwcglxqx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gjaaivesr.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gbqdgfphk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gxcqgddjl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gtdumurea.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gonbtofzt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gcseyecbp.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/guqnbzcok.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gbzbltvim.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gyjvyqvxm.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/guseukpyr.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gzcoykbvn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/getzzvykj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gdkukkrwp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gepswbqap.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gorzgyfle.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/goqhimxut.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gmpfifxos.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gtbulaesi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/ggwsnvhix.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdckpbzpf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gpnaageew.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gviuvaztb.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/ggqpfkxsd.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/grclrsfng.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gyjyssuib.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gmwjvngwu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gyaiamyop.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmmutkre.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/glifchiin.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gpxewkwhz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gtmfbcdhj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gxyqbvgks.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gettljoma.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gpzisileo.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gdeacelvk.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/grwneekuw.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gueynmafx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcpvjbmpu.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gzwckmdms.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gptwrdmml.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gsnntbgwx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gokghakus.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/griubrgry.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gxzeygrbr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/geqdnjfiq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gxeidfiqw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gwtmbcfic.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gefcghhvc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/giobrpquh.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gdhipsuop.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gcsxtrfsk.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gaguisaqu.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gkrwulzyn.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gvasoegeg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gxqukdfgv.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gsgidzcyv.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gszfwjrfx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gkupvzool.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gfanhpwrk.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gjllgfcer.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/glyfrvqpi.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gerguppei.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/grvyrxbcp.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gephloqdh.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gdhelsdem.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gefvtbasw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ghihorbqe.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/ghmdzbscn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gjruawkqh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gxpyrpyib.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/golabbkdk.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gherxdttm.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gjjpqnjsq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwssxurrg.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gebbunaiy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/ghomzfdnk.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/goybvnogf.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gknzmbmqh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gopeopeel.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gnbnzypcy.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gnuyuckat.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ggtgwowbh.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gmcrcsqgh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gifmzkhjs.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gwjrcsouw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gaximmzwu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gncupmlzs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gzmacxgct.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gopxabhjq.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gdnzykcxy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gfdqtnbig.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gfmxwzwgd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gfainqcrl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gnapisips.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gndoeebtm.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gxgrvfpxa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbvzwcdqo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gavaoxttt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gatbpxmav.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gavvsiyvf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/genkxpsvo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gluymqgyq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gotdoibal.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfqcdrqby.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gauxzylac.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gcrpugkqh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gnfdxzwks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gwiopmaqx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gflajxlwj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gliftauii.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gjipxrzaf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gqzkirvaq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwzddgpt.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gwdejsdqg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gjvkpczge.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/grhevkaky.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gpwygnqxc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gxbnotkdv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gwajiwefr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gicchuyba.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gddyiuvdo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gkqzeskkq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gbmxtzruk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gcdhcvhjx.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/ggbtyskkt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gzuciaubz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gvatrtbze.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gsfolgtum.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/guoxjuwqh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gkrmzklbm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gauibfcsc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gszuobvbg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gmgxfyrtu.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/ggxzorrfs.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gnxucunpj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gccwuuchq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gitlfugrv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gsolfyfug.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/govzwmydj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdozwotpa.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gwmfnaskt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gzqpwwckb.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/ghmguehha.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gymqlhywo.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gohhohnbm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gbmpddpoa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goslvbhdp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gdgtjumxi.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/goopifgxd.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gswopqcdg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/glqmwyxdu.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gtbfndzll.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gaiivvbaq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gxuufyjsb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gtsoejdaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqithho.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gcxwweikb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gdroylygy.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gpfeqfusu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gtjgjtekf.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gayxdhbkd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfmechjey.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gajvxdosc.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqhtnoedh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvejfkild.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmtcrfipc.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzucfhagr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gunlqlsbf.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghzsdgdmb.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gagumnpnw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gqdeuyboy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gsewygkdc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gbieugyfz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gxedbskim.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gztsbtxgh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/glflqames.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gknnygdkl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/ghnkaasnq.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gbagvrcus.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gaelsoddm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gwnmvmrod.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/glstqmzof.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gwujfxvsk.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gxjlpsftc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gdotvaplt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gapuitwme.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gqdyqodvi.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gmvycocsn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gmmpdgvwr.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gsmyiwlzk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gylfagchd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gatdmwpwn.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gfgmnffet.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gbtdlwzna.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gpaqhewbt.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gkvczkali.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/glqcnabpw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gqcqleary.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gfudvfesg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gqqbyltxm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gomrzvndx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gdqtkkttt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gtfhiaacz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gprxkcigg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/grnrvwhvd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmtrribvy.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gsawtzhhh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsrdgftqw.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gemklnyzu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gamtzmrcn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gmbieaztd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/guvykkwcm.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gdazvaefb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gpzdziusv.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gfndeplrj.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gzbylzxvh.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gcabqhhxd.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ghvumvqco.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gufrdjtlp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gadoqurxp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gefjcpeft.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gushiwdus.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gpadfmien.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gqcdwtaky.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/grrxcmscs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/glroiejvl.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gbwtplroq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gvugglojo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/grnvvajpf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gmguyamid.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gakfjxist.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gzoncfykj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gojfhdrlk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gekotthwz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ghaxzywsu.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/garjgqfwl.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gslnvfaxw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gyoyzmfod.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gqcgicqgh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gsfraodep.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gvfilsdrv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/ghbdqbrwm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gycieljdt.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gfegfdpam.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gpvogxlqy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/ghhsgymkf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gjpjswcqc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gyzdbyoix.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gtkcmfbiq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gsuqqtxkd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gfqftpxqq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gfxdsrvbo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gvwtybjhh.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/ghpgegugy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gulvsyiqy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gpqeaqhnp.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gsitzyzyp.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gnmpajsur.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/ggxitozil.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gheqtbsae.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gqutsgxfy.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gldhabfsk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giinackbw.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gryavgsax.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grgdwqqzl.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/guudbktao.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gqsvsyajg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gypaqyvvz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gjpvfqgrs.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/goubsyuwk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gkghehnsy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gyuodoedu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gpoawhzgd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gilkyxegy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gomgnaudj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gpehrvzme.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gxuxqbadn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gyzxrodhm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gqrlivoob.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gpmggyrwb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/glztyazvt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gunutovef.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gwqlmlmwp.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gnabjjfwd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gwocooqvi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gvsygizda.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gaksnqcio.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gtmfrjsyk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gjhbkgeud.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gozpczklv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gezblugft.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gpaprhoqf.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ghrwhshit.sHtML


<!-- 参考信息 -->