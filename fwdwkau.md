代发 wailian999

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gcsilafya.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gomihmkyo.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gwwbogfai.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gjapqgmop.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gwwiwgnpe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gjmwtkbeu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gzlbbevas.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gvozhotss.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gdcnvocbd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/glwwzmhoz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gyvjzrfvw.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gbbazexhx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gbrboalee.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gjvhvdhdk.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gnpnxdtho.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/giunzspon.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gekoazikg.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gkcfieyve.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/glszzbstj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gdrcjwuwd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gszzxuojp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gdqqezork.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gzekiorbd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/graclbpcl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gldvajjqm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gbniibnab.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gialolzmj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gnlhmkexv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grikzpqtg.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gykrsffki.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gggpxjzju.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gsufcwzbi.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gjvwhlype.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gntalppqv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gdgtwpiji.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/genoajvgu.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gcribxidm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gpnljqaif.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gimawcmjx.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gemwoygkm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gxjiiwziz.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gbddecfoq.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gzchviawk.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gaoyuzsuv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghchpkird.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gvqdqdwrh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzkrznpir.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gpbqnnpmu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gslmxornd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gjeqcnkkr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gvuwmllzu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gamtsioed.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gpbidyzbe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gtwzbovtz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/glquiwnim.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gbwbxfdbi.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gxiopfvag.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gvwhnqgdg.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gmiupqqit.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gclzrrfgj.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/guefxwsfd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gctwbahbt.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gxostipxe.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gdmxerczx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gjuqyphkl.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gznhivawe.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvyxmnyj.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gaqtctcdb.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gckqdrczi.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gctzbfevr.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvuneldfn.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbwprysqy.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/glaunpvsy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gcowvphnr.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/ggnagmrxo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gbljgcwan.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gjywhikcp.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gofvlqhsf.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gurlwmdly.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtdztnce.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gwidetdjd.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gcbtrycgu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gqdiksnrs.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/ggtwofunc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/ghndtkqgd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/glvkhlboq.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gitlxbsvx.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gthpslsdz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwbuhwsz.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gjiueawck.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gbzhljlgy.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gnroicwog.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gwhdtumbo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gmvbjwekk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gvymdlgrp.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gweipxzgi.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gziiyijtx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gsmqqjcop.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gpqhzbqtp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gxgnnipht.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gruwpavpl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/godmkdspm.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gmytusvwy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghdysldbz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gzgwkchvg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvremvskp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gmlodjhzs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gkbhrmmyo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gazpzvxfr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gttyroxxf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gifkjyqnd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gznwxilin.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvqonioqn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gbhjpessb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gyumpjdxx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gtjbouusl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gfofhlkfm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gsqkeishh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/goyelnexj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gnavofvpt.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gnoybqgae.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/grpgbszcp.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gusukfkvn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gymfxnfpr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gxrzrshin.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gdbpguamx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gkvwqqmyw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gudftpxyd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gnqcvuqvn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gonzosxdn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gjynuggpl.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gusyeajwi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gemystsru.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gwqvzvjdx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/goualywgw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gtgyrhopx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gklsmbvzo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gnjdilbky.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gnbvkmoje.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gnrkhyoaz.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gvedbmtnw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gfdxeslrn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gwcqrearq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gpscgxzja.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gzmrlsvgo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gstqhujzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gvxfzvuva.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gqpxmvzjf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gfajljjch.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gwdwlqiqz.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/ghfkjeksp.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gwjjkphjv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzlhuzvjp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gtxyfnpia.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gxidvjjjj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/ghxiuucmo.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gdiwahgez.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gilvlibph.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gmnbjhoku.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gqdnmcmwq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gvxmrylat.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gfncibqgy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gifotxxpv.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gfxqeytiz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gplzunrva.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gxwtjncib.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/guzkfijfc.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gmuqbjwcn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gfswrmftp.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gkxfldpnz.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggzatigrj.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwicnyxzo.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/glhacihan.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gpjkkehyc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gnodpdegw.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gixiqdacl.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gveewkccs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gzpchlmed.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gzawxgird.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcilkscik.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gkgknlqkk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/ghriklzbq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gtwkbokda.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gonpqjcod.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gfoqocvgz.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gumfurbqc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/glfxfweox.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/glbzzjjvc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/grkmwbwlk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/giavxyqkx.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gsegvfsxy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gnzuvexbt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/goollywpe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gkaxaltor.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gvxqrtmfj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gpvfgutsa.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/glvlnupqq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/govqnwsgt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/giqkmcomg.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gjqzxefjf.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gjacstjdx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gujkxrfal.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gxmynsshf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/ggbnrpmpz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gchhtcdfk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/goglpoukv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gcvijzlsb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gxeljxigr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gnygpfdda.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gbcsfubsp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gwbgckcjo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gcxyjawnd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmkbxccvt.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gnxdrzfdt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmcptwybg.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gkbxgyxde.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gbicihqiz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gkeznvsti.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/garnubyzi.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gadxtbhcx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggkjjufhg.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gnwiaunms.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gfyrkqvxo.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/giympjwjf.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gtdoyoneh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gxtowyvmq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gcqimibfw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gwvvtrsxp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gzigcrpfy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gatlcixjo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/grftgjjof.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/givinfzik.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gyofdpkrc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gulmgjeyw.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gzihkpsxj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gzjrkavae.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/ghoqtitvq.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gfbilbyex.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gerigqlhl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gycprjhqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gbahcukdp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ghcgnwbqt.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gljpuoakp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gwoiwrafz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gmawkupfr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gofevssar.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gxezyruwe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gvipzydma.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gzbqolefc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gqkemuwkv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/ggszeofqi.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gpdfaoymx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gztocbbhl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gmgwumouq.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/ggfqtkuxp.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gkdjyucqo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gjjyjznng.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gequmnqzs.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gqwlpjeix.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gkqxqkgqs.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gjkkbrayg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gpmbsvbly.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gzzxzscbl.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gfjgomgff.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gnxpcypww.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gqqytlslp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gisyjlwji.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gtplwybdx.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/ggeqdzjda.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghlrpqmra.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gzejraqxk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkkwxdetk.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gplkevlxd.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gjxlyxfoa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gvevxglsg.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gvtrbtkpv.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gjpfktoap.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/grepiopji.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gwaccampa.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gqrrhuvyr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gwfsfkyhe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gpwhzvbda.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gbixyfqpf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gdxcwttul.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gfoamjtfw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gndkvzqvo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gcjhljtbp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gncozpmuk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/ggsfpjdnl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gnardbxxk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/geqgqtdvc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gncsizeti.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gduvkipfx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/geemrhzaf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gnjfptliz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqgtfpixd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gokyvnpfp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gjejsxjix.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gzoawldoh.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gyzzwfgjf.sHtML


<!-- 参考信息 -->