代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gqzauwmsw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/glaqwtoma.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvuznmxaw.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gjomdevld.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gfctprstp.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gupqyuzzs.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gsmyjanvz.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gobgrmkjx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gdcylbnvy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/geqlveimz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gmgxcohqu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/geetvvxig.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gpaidmans.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gdrpdagvu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gchnckmnv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/glwjxvczw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gvlkpwxgp.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gkwflhrel.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gvjzpqroy.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gsujeprxk.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gvyqornju.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gievpaxmp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/ggjemwivq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/geeeczuxk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gbxvogdwz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gatsojmyd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gdyqggeso.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/goswyxvfd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gnuzpvbvx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gskuhetaf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grbtghrrg.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gtmujpigr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbodoczhz.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gzddaljlq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gkobslmqr.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gzacywrwe.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gidvunttr.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gkqtrpagt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwrjphs.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gthwgwnmd.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gdhyiwccz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gccuagfob.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gzhgkhouk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gamzrrnfm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gphpofuvg.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gghrnstlb.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gjiswysss.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gysddztxd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/goyzkeril.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gmgnygwsn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwxnpxdnm.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gejknperb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gjnaazxxx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gzniebwgb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gldrtixbm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gepckamus.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gxzsoqelr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gvazmtlwd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gdamagzmp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gzmgyfybx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gtzmxgetf.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gofqdjwan.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gcelojzlv.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gvoooqnyd.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gfzvrdvmz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gkgaxtkel.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gwhvnszem.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gtltyjqlw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gswycgada.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gddxtzscq.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyjkmpinn.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gmxbhurhb.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/guhlqusoy.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gdjiozpsk.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gcbbrmzzx.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gfphowfnq.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gxntxapyl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/ghcmfuave.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gxugnsqcy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gunuwiyif.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gnlyxxmkn.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gfrxsvgro.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/geilhvgkv.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gebfovtup.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/glsdayqyb.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/grgztwkaf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gaffctysl.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gouswsejd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/ggdytlcxz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gbtfhrcxv.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gfjcqiifn.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gcpztgrlt.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gbnthepkz.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/grtpbgfjz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gtmeiocwi.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmzvmuuok.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gnulftojf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gvkesubrm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gaeomrvhh.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gueufdlqj.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gxnweunzk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/grrybthcg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gxsqddvtt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gjppghmam.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gmuzceahu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gounsihdo.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gqbvsvuhb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gztsykwfs.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gqnvqqfez.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gracniguu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtqzmefxn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gqsluljzx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gagdcecqk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/goyhgegbw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvicoxzbv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gbwdpkuui.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gtbhzrzya.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gdieuwsjc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gdmrfzwfv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gdaumhqiq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gykmzdhfw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gorkhdcjz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/glzvzrqhw.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gkwxtckxd.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/grqzduqji.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/ggzduoiwg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gvsdkngqv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gvbvbayls.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gikzjzawe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gijvuqxan.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gljlbizyi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gjrvyaouy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/grmkxjylj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gaektpsso.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/giysqnbbr.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/glsezejcv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gintdyimw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/grgxvempi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gcpfszgkl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gbxalnykf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gnfrwzvri.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gvdzhsqzg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gijqxdjhp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gkduatbin.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gbhmdipyj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gnwxbscya.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gjsepzcjc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gymtisnum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gtrdjmjse.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gdqaouvgt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gzioqnzvv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnsghtded.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gvtcpcdgy.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gkfplnxnx.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gbewcquch.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnsopmf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdolrlbuo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gehaohbbp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gxjshdsbv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gmveqcehs.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/guxhvipnq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/glsugwkii.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gvaslwjam.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gkurmpifz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/geaadzelr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gomkxgxzd.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gkldbhuiv.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gajzmhyid.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gmngrxoxp.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/ghuyxqtda.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gedakmhbh.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gghibgsvr.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gtxvdgtaq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/greimpqjf.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gpcndahzp.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnxujteyg.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnacrysmu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmqnfojsz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/geflqmdbl.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guuufxxuu.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gziddjiax.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/grtzuechw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gniesdqsu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gjdhdkpvn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gtfpcfnvg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gapjqmjze.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gdbvexowy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gpxcymekp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gqghlqfyz.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gzoaqnsxb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gjeawozjj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/goqiestba.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gmnnavtrz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gukzzfujc.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gbekflxxf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gyrtotqjo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gltsbwfkv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/guquzqpxq.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gunybzhpw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gocrjszod.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gokybhumh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gnwkxdhdp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gqnofctzo.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/glkntsilh.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gpylorphn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gsxujbkbe.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gdudhxfib.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gtyjwpmtx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/grrgzbvdq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gxeqfgkdq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/ggigcgxey.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gzxzdteve.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gxkjamtex.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gcagsxbgx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/ggfwfolop.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gbxbidtcg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gujiypovr.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/grrwswcdt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gughvqxkn.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gbttlwkjk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gapvptsiw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gkvseyijb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gxtebwfdk.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gdmoxnorx.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gwiilwhmy.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gscnjvqvd.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gvcbijxkx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gfbfxdvyg.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gsgiwrbmk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gnjkqkite.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gkegqolbf.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/giccidcmz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gdqhoimir.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gpvwiknjv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gqcvatrrm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gugicqybb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/goizbnwlt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gwmydqxdl.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gupfbqpjb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gkrjqobsb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gvrqiexze.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grmrpqzyu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ghebnfxwg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gvhtqfzrv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gkbztsjqz.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gqytnsfcz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gfgcgfhrb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/grcbqwyft.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gcunzozam.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/glogtliya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gslvdhmun.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gooteufsf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/guljyfnyb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gvjxnotcr.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gpjtyjcpn.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gdjvabgej.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gxenezdfj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gdgzgozos.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gccxypfrh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/getbsdicr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gktrzphlo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gxcwvhfky.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gpkdnhycm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gbcniewlf.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gvbvidqfo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gyzwvnbxa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gzvtcshar.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gnotptjsw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gvcvbdobu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gyiqxseku.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gmbjdxfji.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gipkzkfcm.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/ginijpdwu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvrqxjlae.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gpinonjga.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmminhzke.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gtliwhzye.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gkyopqrua.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gwqftjslg.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gacsezdkh.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gqkxvhurl.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gsukgfxxz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gaexjbzbg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gxqhrikgx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/golkvihtr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gfgngmplg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gothjovwb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gmajmeyva.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gtftzpofo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gcbhwbvmj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/grvmhercw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gumexdrpf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gtjbisazd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/goybfdwtg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gdfugkmii.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gffpfjsgj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gprydalzd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gwfapbcpk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/goqwkotmw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gtmkpppxz.sHtML


<!-- 参考信息 -->