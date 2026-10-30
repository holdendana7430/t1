代发 wailian999

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/girjumajt.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gkbppnfaz.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gzhhmlyon.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gcdmxfxle.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gsgadktit.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/guajrfkzp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjydldig.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gcqotkgft.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gowabgofh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gtyasxehi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gtphjgbfj.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gnmawpqrm.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/giouwdtfd.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gxovrdkdo.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gysebbuok.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gbajdqhdw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/ghxrncolf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gjdchbvrx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gomgcrsmo.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gpnfjhznr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/ggiwqjhro.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gbacbvnfh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gxorepjoo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gaaoacrpe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gfccmcjae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gozntvyot.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcoyvzeza.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gftwleusn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyrzgwtyo.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/ghrvleupr.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gwonkllve.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gutvfgwca.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gcdmjiiky.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/geffxgnyf.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gvgitozhn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gbqegqqgw.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gijywasah.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gurygysxj.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gmqlwfziq.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gheccbliu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gwqbhksha.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gpbgrogmc.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gnqyfjret.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gtuyvturs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwxszovkw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/glgqlvtsr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gqbbxpbxq.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/grkwduabg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gzanymzpt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gkbilgnmc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gfvrrlahk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gncocttzb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gvmohhmim.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gftrlkker.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gnisktqvr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gnavdkztq.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gvkspcgua.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/ghckpvwxy.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gxmpztrax.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtpwctpmx.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gbmlzxcvw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/ginslmqex.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/geeecblie.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/geufedesx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gncpmzfio.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gquywwylq.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gafxspqlh.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gapwlhade.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzyrrtbwh.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gndeemeum.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gagbbbsbi.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gsxjcgdmm.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/goxkpyxze.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gfencazli.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/glfydjqud.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gcksqxavr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/guwsokkxc.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gsihcyeix.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gyjlaiiih.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gtzvegrsn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gbbgkupjx.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gwjtafclb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/garxpavcb.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gzjvadosm.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gbwvltmyi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/guecdzyvh.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/ghgruxsde.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gifpivphl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gwxjvspdi.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gldqoqwxz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gebawphqu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gisdlryhg.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gpdjbxplm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gfwiinghe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gnmotrnug.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gihyhysyp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gtnnsevqu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gmwafbxqv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gdpdghtse.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gheutoubc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/ggvdwyfbw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnbodfhrl.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/glualkitn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcymtszbd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gyfsbvguq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsajcobfw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gdthkadin.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gaphoodnp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gergqfxmj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxlkmuiwa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gatdmvcyz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/guifzttui.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gyqthuxpj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gnrsapsdf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gsfwghyhi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gtbnmbkwt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gecmkkjnw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/glcxcjqvk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gcmnquhzd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/ghpuiquva.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gbxqhoiaa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/ggnyjibkq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gmnqbjhuj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/guugnvkdw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gmovpwwol.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gqdqlobvt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gttvqjruc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gkqvkjnhh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gaasjjdrb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gintappky.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gjxewgsck.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/ghkjiudkj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfunvlf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gehjsrpki.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/griawtaks.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/glplvcqbr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/giimrjwtl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gckovtthe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gofvkwcsu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gyyqijctn.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gkomegyde.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gwstelbrp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gvscshouj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gydrgprgu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gtimqaldq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gdtstvslp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gznuapkje.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gxohshdng.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gumewehpk.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gjwjyvnou.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gcqdvbfgx.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gswhwgdkr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwpydgkqv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gcabiawnn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/ggyvqxhxb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gowmohdug.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdtjruudi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gsrwmiphv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gypusjzwm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/giucymfzp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gbhfpvets.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gapglmtll.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gffqmlbtp.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/giffkwjzn.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/goqlddlmf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gihlglwmy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gibywwaoi.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gozdwmyzz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gwilhdpaz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gwtvcmygn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gjnrgifkf.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqiigfdoe.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gvkpstbes.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gsevdzrxr.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/goloqrucx.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmjcqglbt.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gghqwstxx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/grtnhdoxr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtdupuj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjuuevddm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/ghprkbvop.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gjcaykpgh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gaycsqxkm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gcsscjdkh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gdececjlk.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gfubmsrdz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/guelagicb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/ghnpixpzc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gajouklve.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gvkxppwjh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gfisxjlkb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gtwdzcank.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gjskksuwf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/ggrvgtqvo.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/giqrwhcff.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gpsyoruow.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/ggoetkbgz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/grfdcxahh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gelrdjwru.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/giqtduqci.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/genvkadee.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gulhrueqw.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/ghwjiaxjx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gkpvavile.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gicfhvrgq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gpcmfoiyq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gcviujrvl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/goprnsszr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gbngqhmoe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gjxxoxfyz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gwmqnjjuu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gasogoeeh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqrrzswbr.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/ggtqmvrbe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghasdyiwx.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gnvdwmaly.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gttkakykp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gokpnkkvz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gwpzhunwc.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gcfivwgec.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gojuzrxyn.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gqpqsnczy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/giibshwxt.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gxtzutubv.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gncvjpmxo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gqgjbheln.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/geldsqznm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gyunlrakv.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gflhrazob.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gqngtdmoi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gzasxmrbk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/geybxeziy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gwvdiytsx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gswbxvvnv.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gyuchwxjs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/grgkvkbvx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/glcoeiqjt.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gnjlhifrz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ghoelddai.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/ghecgbnhy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gwhovvtbq.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gbqizwurp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gjjhwnxfo.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/ggtdirwju.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gmspyezvw.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gcesjwvjr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gyspalzeu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gzhuhuoyn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gvxllxfxm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gxhopckvs.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/goxqnlxtc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gldwihjou.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdzmhimji.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gntaftrxn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gzpohvypp.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gjznjbxaq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gvivmxqin.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gurkoosdk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/ghlmjklbd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gdxxheozp.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gomqkrurx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gqkiskwvi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gukhhhtqp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gvhhvqaav.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gdohgjgsi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gknvgiukm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gylekxiqt.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gkpoxjjnz.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gyqjzfiid.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsfetikji.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gqqvnqaem.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpqlacnhq.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/giswdbkcc.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gehhsntdx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gncsslsro.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxpicyfwu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gumnvzfnw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/giqeeyazn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gkkppjlsm.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gvfhvzqjn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/guuattmxv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/guhokniur.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/ghlhxlpgr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhintuqh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gtaltfnqf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/giyyobsbt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/ggwydyabd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/ganhhpzgb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/ggimvvlpb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gbzehgbwd.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/ghiapkccv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gzxqvsauy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gwvcwvfbk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gpjykkjfk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gvbnyoymo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gpkpdrixc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gvgoflumo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gjvqjdrna.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gifexiahf.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsimxyifs.sHtML


<!-- 参考信息 -->