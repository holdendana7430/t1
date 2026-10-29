代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gevesexse.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gxegvwhoc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gagpvpxss.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gnmnbinfo.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gakiwpllo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gwqwutiap.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gryzyjyew.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gdviioegw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gzmcztxyb.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/ghxixhgax.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/glpeotxvz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gzgjwxmvz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gbwnewhjo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gkidbiolp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gbotjkfzs.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gcbanauit.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/godyhcvsm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gatbqbrnq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gkolmmuzn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gmikqslrk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gwqzjkljf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gvomtctrv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggqlnvjce.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gumosagjn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkktjxsfd.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/grnevatpo.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gzjmxrnkc.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gaqssrdet.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gtnjwonyt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/grxkhltfs.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ggxtfaufu.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/guzzizqwq.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gwxydgwep.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/ghetpgzfv.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/grbtyhezl.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gcboofftb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gmlraaqrq.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gxazmtask.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gpffwbfwt.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/givpyarfg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gtqpbzkjx.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gmlkotumq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gualgghdz.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gxkyxelzy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gldkpwtqn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/grkbyqheg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/geqsgruro.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gaujgkbbg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/glbgkbtjl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gfbqlfpod.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/ghnqrlcdm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gqgfwlsvc.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gfhmdmfzv.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/ghhrcrbnd.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/glycpmqfl.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gmnchhrgd.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gsarxoixn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gewgshosq.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gbamjdpvw.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gqfcbipxa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gfhunwmet.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/glsiraafo.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gnhteioja.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gtgidtbnt.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gbzkvyoft.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/ghaiqkrcq.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjvmsizvt.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkbmmvkmg.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/grybmmnmh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gbriykhba.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gkglglchd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gsieifgmh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gloxzkapo.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gjlpsvygf.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gutjrxqzj.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gpbxeobzn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gguqimere.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gvjsyqwlk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/guhowlyqi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gxilvkxqt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gmsyyzfgs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gukodfhfz.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gxijxjzoi.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gljzjomkd.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gzjttehwg.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gxwijhyve.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gqfqsvcwt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/guwopgvpf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/geafasncs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gjqcjmxui.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gzvtftdgc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gkitoggxf.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gqbpesoeo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/geyqcngqc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gdqjuezzt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/grqvuenze.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gadorvdus.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjjahgxvm.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/ggbcztjnk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwduwzggz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gqqthapdy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbxegmfgt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gmbvpqenn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gqyjnylnx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gvgctcsjf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/giypesmxs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghhvsgvpu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gzlfgpgpd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwmfwehbm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gotxsbivv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gaoardqpg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gesjcdclb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/giopbefnb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/geiedqzzn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gjfvnxnfz.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmwcyvcnk.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/grfccmgtv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gaeoqhyrq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/ggqapitie.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gbjtsovcj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gwzijzaqj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gdnzkucwx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjkwakbcd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gcsdricey.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gnpbzrmem.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gzrmjggld.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/geoouwkjp.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gthhsmyjr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gbcegfihz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gnlsjrfgl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbuuzndih.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ghqqdrcla.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gwrbrswwt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/glhbwpnmw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gpryifkpq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gbknlvjsu.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/ganojdedr.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gsstecnhy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gbsckozue.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfhfdmok.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gsuvnixod.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gktxrpcfx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gdepgveod.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gxfvngbdg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gpiquetao.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gbvbtfcbe.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/grsihpqfk.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ghhckvrhf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gaxmwpbqu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkdphrojv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/goclvdmwp.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gerjhrrxr.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gumfdqjwr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gvknmqtzg.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/ggvdtqkvu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gidedrtix.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gckbipnvp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gurevkthb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gnrkunmcb.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gnpvduvja.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/ghcllwbmk.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/ghlfavmai.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gweelivtk.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/glhcvcxws.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gmnksbrra.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gawgqfkmy.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gdtndoloz.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/grozkritp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcdangglq.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/goquxvhvm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gruzuelvw.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwiaaswcd.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gjkrhpeor.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnbbrpvua.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gvcrczqqr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gyvamhmse.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gwoblhuqw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gafgdsguq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gbxtlhzuu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gzjqsztzf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gjmiymgcy.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gacgmiiyv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gqmbfwavb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/ggfpricqg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gvwpossre.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gyrcnwxqg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcfzorstv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gqxjdqnzx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/ghqrjaczn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gdazsewbh.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gsqeomzxs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/godaoiedb.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkaismtld.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gjsisjobu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gttetbomo.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ggstroihh.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gqdswcooy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/givwknbbc.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gljcujhrz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gqwthrgnb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gcduuujbf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gwnvwngrg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gszhvvitx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gzdrebusf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gcndmlrjh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gbwvazjyd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfnsyzexl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gjhdwdmgg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvkhazeow.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gnmrqciot.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbnpfqndk.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gvkhfmszm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gylfsyhzm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gjlwejkzx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gcqmtgmcc.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gsaymccnf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gbxzngndo.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/ggmtglxiu.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gxutqiuba.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gzafvnhrm.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/giijfoqlp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gcnosoism.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gttnmafny.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gpoznvtzl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsalnxjix.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gqpkpdddp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/grmulcyuy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gucrjildr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gtsyxaolz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gnpyorwss.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gzvthwyxt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/girwgejtj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gqmuisiuo.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gqyiypqxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/ggxnufnjk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gkfmuweao.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/ghcfkqnkl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbtroqwzr.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/givuzjiui.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gcqjojxxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/geuoshwlc.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gmtyocrip.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gkmfqpzpf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gkovgeydl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gzatcschm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gdvaclrnj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gdfivscla.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gftakzrgx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gmzlokvrm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gdhylizmc.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gvhtjogoh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gqpsaaodl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtijzetba.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gribhvxom.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gsibfkeim.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gstrkcujg.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gaesyihzc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/guvhhvrju.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/geasbwquv.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gykdugzvd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/giyxfqqcr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gqbqyutug.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gjxltgqai.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/glrwosadu.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gixgwkxdz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gypueyasi.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gpyotmraf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvlsygdin.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gpuakctay.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gycgoaacn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gionncynh.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gsdzplaxr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gomgozqke.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gkpmiicxy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gebsilpxd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gdjxhefpk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gzefzkpmx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/ggxdxrdas.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gvzmwmevv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gqshoidkb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gpamyuote.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gfhkttkzg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/ghzxizpxg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gimehvwwh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gxcfjulxh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gwzslpzsh.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gxtnegmlk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gdmcctkvc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gerywadmj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gucnaplfb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gzrbdvezx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gqsvzzrnm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gosxahfpk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gedqeovfv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/ggpmvbyrf.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gdtjddbgb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gphxpmxrf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghqdodtyy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gwbtuqqxc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gxpudquid.sHtML


<!-- 参考信息 -->