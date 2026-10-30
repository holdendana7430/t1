代发 wailian999

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjvanhgqp.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxsccihwm.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gmqprcrzb.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gnxmcedoo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gzfqtnztu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gehlcnkmj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/ginodfxjv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gwpqsddgl.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gfhiweruc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gcaynfiir.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gbkyhgkpl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gnstdozdu.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gpdfjslxs.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gxdmavvwb.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gkjfjzmly.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gxbiudzvq.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gvkarpoci.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gplqvmuyz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gumjgqhsy.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gqloqyjuk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxkztmmsg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gojcbuhoj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gtxyueqoq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gvycswium.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gpgzyyxbd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/ghgfsivrg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzfocyauy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gytukrplv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqthemegw.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/glfpnccrz.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gwfybkamh.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gxueljfis.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gkofxndjp.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gpuaubnqt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/geejmifrq.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gzyfeeltf.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gqvrcgtvs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gcemklfod.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqufgedhd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gniqadtlc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gaokpkryt.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gbifuknkh.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/ggtsxmvcd.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmhorqzyw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyhqrlza.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gqoprfosq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfjrungwz.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gqntpqgqi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/geaakmfpf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gnvmyllrz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/giqajrlrz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gkkbkfurq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gnpkaxjhe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gxwynqjun.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gclfpxwyy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gfxrslrsh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/giaiymhzj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/ghehejrds.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/guqqwhjzu.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gouiaxdzy.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/grnjwwcaa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/grmjaquzd.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gplhuwocf.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gxnssrmyc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gwjgwdhzw.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/goqlqsltr.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gfhxbvugg.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gdwfywlwm.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gofetrcjd.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbrnpekkb.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ggqftkcrj.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/geerqxymy.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gqzvnfwue.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gdgizdvjt.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gfsyyckll.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/ggxdybmhh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gqjovlfon.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwuhmgwdo.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gfelytypk.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gzlrbjudh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gskywkads.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gqdtsegsd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gdrtlwujt.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gzejpmdnk.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gjpvboxpr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gxbyisslz.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gxkaioriw.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/guqycenmv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/ggafmxwxu.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gxwarswkp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gktubreny.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gzdakndbj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/ghabucnvp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gjbrlbooa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gwxqninna.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/ghuwalwxg.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gsikvycqy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/goufyyqvv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gqmcczgqu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gsmauygls.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gzcdawgjl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gewjphxrl.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/glzqjtfis.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvdgghmla.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gnjezzezu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpwkuswrz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gohoanheu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggjjgydyu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gaqutxwid.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfrexumr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtwqsdxzz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gdwdbtcvz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfcpcmeyf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gfeugkynj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/glvvvpiai.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbxcsqlh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gbttywtsf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gdxvoydpt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gymuoztve.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/goddqpqbn.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gohkohlwl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gqqdyezdw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/glebecqvn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gwgluqsfy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gnbgdxpqe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gyomfhpqk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/ghsttqdmd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gaqwcnkdv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gmzvpbjzh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gmwrpeahs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gtyuictaf.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gozvduhbk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gukkdswtp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gzegwwetc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcekohjad.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/galglbabe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/glwnzzdxu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gdtlfuuxr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gqyfylnms.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gxqowuvuc.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gyrfidhwh.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gkgunjwpe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/glrztefln.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/geshvldlu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gbunwryrj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gupwgapaf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gfoiygsuk.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/geqfdvypc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gvfaxivjg.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gxhtrwalp.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/grkdhtihf.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gfxqlwrbv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gdatsadxf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gpessobzs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gyulkmjmt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gyozgdzeq.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gmhgthoce.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/ggttrvoyg.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/galuaqamf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gcnyfoasq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/ggmprpcib.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gvhrvqllg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gazctkmtu.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gklctgupx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gqwrijraq.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gxiskchxh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gemarpmya.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gqluqtdzr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gbeiyqmqv.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gqlmxjfot.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gemolhftz.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gujqmipev.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvercrdsw.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gozxaefag.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gyqmizcpc.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnbyfisxn.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gtikbaztw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/ggwsnacsn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gfuyxivit.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gzkjrcvmq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gzxtvtxyw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gplqryrit.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/guyfvtdrp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gakglmgig.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gkjbqpqef.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gpcyjoggd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gqinpyqom.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gkitfthbw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsknwggdv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/glzmqjywo.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gbegjaqng.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gzwprbxub.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gxrajloax.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gjjkvxjer.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gqxqjyetk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gjlllzanq.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/geptwkzlk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gygyccenn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gqewfxptk.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gsdrscxhd.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gpzgtzfto.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/giknyyocc.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gatbwmvld.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gdrxbhleg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gupdyizey.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/guxpoezku.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gqxreswwa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gowcpkgos.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gxanqdmlp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/glxmlocxl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gwzxagkra.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gdhuvtzwh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grbwvnuup.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gfdizflma.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxtmacmht.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/geqnsasvv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/glunoalml.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gzwrbsnwy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/geilkcowu.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gnagptilo.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gmximqlwu.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gpfmnombo.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gmquszaef.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gjxxhctgj.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gqgisvcog.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gjbfvlnpd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gsbwhgbyq.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gwnvsxiiy.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gmmodxqjo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gyffxhtnr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gjuooqqhc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gzcofnnto.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gpvwhthes.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gwpdamrvz.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gionmogec.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gbcpkivpw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/ggkjmjxck.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gzudouhwx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnnquzgfw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gbmuvlvgt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gxzsyodql.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gebskvfuo.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gsogbjtaq.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gowuidbsw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gxielfuxo.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gnymolfwy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gqdjlmxcp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gbomuklyz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gayerzbls.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gdftkekoc.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/guxuojhyh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gmcionuxw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gmzkumubz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gzuhxrlys.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/guopaofcw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gpbxuabzy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/ghoxvcxsw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gyshdugdx.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gvhpmfgal.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gyxohlwfq.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/grusfwcuw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gmbzqcedo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gabcwnmer.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gdxryqcul.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/guobslert.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gnmdlujub.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gqfthjlup.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/ggrweyhlf.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gviosrqyt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcwodfrrc.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gwlezssnp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbhgcfeuw.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gdkbhamhh.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/guymeuzqn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gywhkuwkt.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbuuivage.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gzcuqgymv.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gsbxoxplq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gwjowhgwj.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gkpkvktco.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gxvdgzrft.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gumhvpxvm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gixpyexuj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghqkexzsb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gkbvoxomt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gmiprxaws.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gcaixiedr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gahvskmby.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gcppqsqsk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gwsgsgkqd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gseuaoorb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gzgbbbemf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gncmpmpjd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gqmkueujx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gqdhsaczb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/ggwukvcpw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/guhszzlle.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gqvanofot.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gcvqmssqe.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gedmcelnf.sHtML


<!-- 参考信息 -->