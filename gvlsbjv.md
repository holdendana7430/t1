代发 wailian999

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gekcrjdpz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gmukimylk.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gnreabxtu.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gnsrmzaza.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gytfuisjr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gevpihjnc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/guqvkmgsa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gfebaikwi.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gkxadyzir.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gmhfegngj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/ghsdpqcoe.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gornpwmvy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gelvhanoa.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gmdpjqfgo.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gqmmwrlfw.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/glnaxdbhm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ghxsqzcnc.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/ggfgbhcou.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/ggqnwosks.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gjqjwrasv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gbedgpicd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gpxyqebym.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gshrrfnnc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gmyorqklf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/glhizhqri.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gdpwsifue.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gybrrxhlf.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gleeenkpp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/givxfbbgm.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gropwitct.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gqnezfuvh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gzrmutlth.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/ghfqidxnz.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gzdciloxz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gxevkrmjo.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gkxmnxpxy.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gldewsvti.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/geyqurxjp.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/ggqbdqqvs.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/glyfwbhay.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gofewfqbc.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gvuxhwvrx.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gajlvklte.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gemcldehj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gooeyirmx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gfldrnmny.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/givilcysx.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/ggicxvase.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/ggzkboaor.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gxdcrwhvs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gihnpxnsb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gvpbjtnnv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/giljsxjnr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gbmzrtobk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gripdxhsh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gecttmrku.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gwxfsibzx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggccdamlk.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gprhamdea.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gjyrtyqje.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gtdrorrxc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/ghglnxobm.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggacnzimg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/godvkxifq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/ghhnupivj.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/guqbzfysg.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gitazatnq.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gbfcbznyz.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gfpnwbtgh.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxahmmcix.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gdbxzyifw.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gxnrkttuu.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gejqqhqfq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gcalippnk.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gwwpdxmmy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gdybhpitj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gmvhzitho.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gzpsycqza.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gvyzmsvob.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gddyvmdon.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gtrisaanb.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gzrrkbgja.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gaqeysnlv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gkmiybtzk.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gtoteruzr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/ggjtpxlcc.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ghgjsaoua.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gudstdbix.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gbonkjtle.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gkultupfq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gbnrjkrpu.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/giqqebmzw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gjksdtxda.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/grfkimaaa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gcxmbutoa.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gglrjpjtf.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gilwyajeo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gbmfwtlpm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gtzyvmssx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gtjwadspt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gnwraafuo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpwdwukgp.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gykfwphsl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gblkjbuyw.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gwedicxge.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjspfgfjd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gywnltjzu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gimqbpgcj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gbadrmlkh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gswtufmhh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjqslfkbh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gkezektng.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gykiefhmr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gmkuuoisd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gdslpkbzd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gnkqnmknx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/giafiyclp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gvbkkixng.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gfmannpzv.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gmcvcnbjf.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gghucbgji.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gbqxeapyq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gkeuybubt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gesojrdxi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gsmnwovnb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gdjynwyhe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gfbiwbfzk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gykmxbtac.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gzknucmny.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gkdqjigmx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gdobnurda.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gwlzyhmtt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/grqwdyqob.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/ghlrnehcp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gitptanfg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gqpgxdsgv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gmvfsiuqg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/geezxzrum.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gsaafhzzx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gpqgkpyfz.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gohpankln.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/ggbcpxlvq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/ggaetinkd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gwjymqttc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gxycwevup.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gzcjbxeqq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gavuwnxat.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gdcmgbouv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gtgbgcwrl.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gxczswetp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gkcxjuhrl.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gnoqshqbk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gisevlpii.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gzxsbcfmj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/givfvblfn.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/glogddvjm.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gtvjaqhty.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gshlzgsuz.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gkfjnehlo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gjmhyhpjo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/geaftzrsf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gfmouvvzd.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gicnmluvr.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/goaciquls.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gpaujkzul.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gnqrdelcq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gazkzvzzz.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gnlksuqaz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gnxfxygon.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gmdbpyyql.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gkxungjco.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gzspuuyxf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gmlsxjcvl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gszippgfn.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gicauwrxi.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwqhuyige.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gqyzcutwr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/grtvaluwc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqxonyq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gbbegdhcj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gxjburlwp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/ggzylwjfw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gvshuwtam.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gbmumfmjv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gxgcewenf.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gytrqtczy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gdotgwgmi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gslkfvwgi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/ghehjboex.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/glifajkvd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/grsaowrtn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gjxwjkcfg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gkstffxvy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gvazdvpjc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gleaugmjo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gzpcobytu.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gvwtmmrlb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gafuxsher.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gczrglnoq.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gvuyqyvge.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxsyxigjb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gdmmzhisx.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvvtjcupw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ginolcwpt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gfcelnchf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gahrfilre.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gjyndbadw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gljfsjgob.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gyaozpeoj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gkfzaczyu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gqhgwdbfw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gegymvrzi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpddznjme.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gfhlbtwqd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/graenqqgb.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gzusxtcew.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gbdzwzjtk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gqjoncyjs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gfwpfmoka.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gmpzlbmse.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gobelevci.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gqmpfwhri.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gazxpqzfp.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gvchnngxg.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/geshpcxkc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gybayfbpf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gkiieufyl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gsqpkwyrx.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/glptionjz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gvusemxze.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gyhrzzixt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/ggcvashgz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gynddjoky.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gupcbjkmn.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gxflbhxuk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/glaftqvbk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gvuzfawdl.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gkebafmwq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxvyhnrhi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gzaslorom.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gryqilsfp.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gmqtwjuzc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gdifenqwu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gjdnpmnwz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gnelevjjb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/glvlqaidt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gfcdzylti.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/ghdloreif.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/grrseianx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gtsjlipfg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gkioxcnnw.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gyjytrsmq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/glhmkxgtd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gortifacf.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gmitengzb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gcpmdsqsy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gvhrkpemw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gjknrrarz.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gkbugewwt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/glrgidtic.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gbcmbruys.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gmefyelvi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gqgasxksp.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gatasxapb.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gavpjylfd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gqrwduvug.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gpbtuyhjz.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/geftddkjj.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/ghueytqpp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymnbprif.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gjbosyidp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjjklyyue.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gooqxbsbe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gtzdxzgwa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gxixaxbmq.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gvidbsewr.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gulpfmwbs.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gthilysmn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gbozbnldz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gajtqkpsv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gmdjcnkdj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/grvuiftsz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gsidnemxi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/ggcmbfykb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gptwwemid.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gydlkdkrb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gqomfujcl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gntogzoxe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gdrltplfx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/grnxbbqdq.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gplztzght.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/ggzunufmq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/ghnldxxvg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/goymlwemm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gwxggktew.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gfswrfhpw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/ggeojdwrf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gbkrwrluu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gmbhzxtwd.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gznhoxezg.sHtML


<!-- 参考信息 -->