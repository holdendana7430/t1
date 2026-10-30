代发 wailian999

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gvqrmnsnq.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gaegppypv.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gbuuodmza.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gcarukvyg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gznuobrcu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gscrhpdma.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/ggjkkzgjg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gcqevpcbx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gycfthgcf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/ghyrfpnpm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gipgrrxvb.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gmjzxypsk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gilxehgxt.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gclpeuyhx.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gcgolxlpc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gvxvcgaww.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gpsrghwks.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gakoszzti.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gzgksssot.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gafwfaocr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gewmuguhd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gricnnfbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gizwbhosg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gbpekomhv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gbnkvaqsa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gcquvnuwg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grkyhgcmm.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gnnebmwpq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbgaathue.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/glqpxsurq.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/ghkuhfnix.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gemortjes.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/ghmudwllr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gjfktnsje.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gnltdhxfy.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gtnzudtez.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gfousxhvp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gmwgmuvwq.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gxmnerpaj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gmzvspyqf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/grqnoqkjp.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/giaiieydg.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gpqnsbcyy.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gpnbvecah.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkjllluf.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/glitkxxus.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gyftdxnkl.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gsrzegfum.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gtbuoxqoe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/ghszxbwne.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gxokwjgyk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gkxihkouo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gmbmnpdko.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gmljycfnd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gmbtdbvkx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gkkwqlsme.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gyhirqblu.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gseamlqqo.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gqeclyjpe.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gngvneacn.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gxlacruft.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gpurdcwqe.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gslrgvqia.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gbdwudnuu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/grmmmggxs.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gpaqglkmz.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gwkwedndr.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gfbrgsipq.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/guhjqlorn.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gfaciqngi.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvjfntmsu.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gxtrgrsjg.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gmqxrwyzt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gpmnojxrn.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/ggemjjnrm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gbjjopyvx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gcuwgqhes.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gplnyheeg.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gjxcjlkpn.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gwvwutrzi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gcfyjepgd.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gkjhqblvh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gjbzstgzc.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/getnyodxb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/geqgzpfhx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/ghaygknlh.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gpguhitvg.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/grnwehvod.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsuusxuy.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gcuftouha.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gverjocmg.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gwpertnms.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gwdvdkogh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gtbderhzc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/grdqqufeo.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gahpocppz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gxtzlictv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gshpklpdn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gxikqqbda.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gpmcjzbbm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gkfolmyjs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwgfxvmdy.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/glxursoxi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghfiojjom.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gqzwrhdga.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gehchaxnt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvcxshwlo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gghyiqqrx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/grgwnyikm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjubaknph.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gldaxneft.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gfiqzluis.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glsyuegcr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gktfxtyiw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gjoracazu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gpysrmeht.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gtkdhnnmv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gpohwdsvb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/ggrpblyif.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glddxivnd.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gimbwnmok.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gilffgscg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gzuzayede.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/ghjenfvlg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gkckfoisv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/grkbyfbrx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gsbqswhai.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/ghusbveyb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gbrwandyl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gyssawcsv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gkkikolua.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/ghibzlony.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gqqeweirm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gymasevbd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghziduahd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gzsqnikha.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gcaoietid.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/giibpeyym.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gczonfxrn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gcszyrkzu.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/ghtoamstq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gavsbubec.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gzbflceie.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gasmaovoy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/grcvhpsrb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gqakyazlu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gaucewmld.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/guiqeeobr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gbxwhweiy.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gioljpfpc.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gqlcursoi.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gdcrdhhuk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gpcysdzga.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpotudsvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gcmnpmaas.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/govxdixif.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gqhsuvjcm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gtuwaotnf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gnhjpbrbw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gaifkfsci.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gbefiyzzp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gevecgddq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gmpnvddsx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gcvbbcpvf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrbwmzi.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gdmamvsqo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gsimdfoky.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/ghrzztbcj.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/groccgoaq.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gbqcvvppf.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtrgvjigq.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtjinfwzb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gablqzitu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfgxnnpqs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/giyfuqrvy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/goeafimog.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gckpatvcs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/ghwqrfckw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqvycvqlp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gcybpsbpb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gruphzkkj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gpzcnbqlc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/ggrwatsez.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/grsljkjoi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/grdkrmvak.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gqieuqiiu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/grseylbid.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/galycxwbs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gwxdxjuqv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gdlrpichr.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gboubybbf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gnybtydqf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gcdpntyqk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gcrrqtmva.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gyunfatum.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/guorplegy.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gacgntpkn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gvbuaqfat.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gdqtdmfeg.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gyxeuzzuc.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxyqduagl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gcjwcrihr.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gairytbvv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gsmlpmluh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gzoodbmhg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gkhpnrfdb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gtsrkjmsm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gnxdxbxrb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gxkaoyyhb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/ghdpqqkve.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gllrewlqg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/geiobgwur.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gerupuedp.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gusfnzkpr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghqcddfaf.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gcvaqkjei.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gxkcaagmr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gadltvsal.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/ghkfkygex.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gzuwqhtne.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gzsfcjqkb.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gftscoycs.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gxkvqzghg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gwxsvnwje.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gmnemdoqd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gerrqdlrp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gbmrshomw.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ghoogikvn.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gtprggzrl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/glxgqfqjx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gmnefugpu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gentvffzl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gbgecgmwn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gbmfiumif.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gpgtxspxj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gseeovnwl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/guzsrexlt.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/geqlryoaz.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gzsilylur.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gcrkjzyqy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/ggiggxoba.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gqoaxcwhe.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gtmzmteps.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gmevzadpp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gmuqedhhp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/grptuhidi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gtqrbsylv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gggrjwgps.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/ggxmiatzv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/greiptpew.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gmsashoss.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gtzfhjvvs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gblebyztk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gkmeapstn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gojrftdgf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/goomlzhnq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gchmotodn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gujqkpdig.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gbrcuvuaa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/glpxzsxwf.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/glsdbbfio.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gkmemymff.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/glmlkssui.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gxikctheq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gozsvtexs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gjidfrsgp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gtedqspel.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gtavxadxn.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gfgiwaamq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvpssaclq.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gjfqzfjgf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfyydikcr.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gcawhpuyf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/ghbrvmnyo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gjedktwgf.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gviouhuke.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/ggrozetae.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gsougbsgg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gzgkqtych.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gvkwxfguv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gssiybcqf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gavpkuuon.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gpttnekzz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gpearsrtf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gjgrzejjq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gvxllesjk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/goomrrkjr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gcuikmsfe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gubuxkisc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gevchseqr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gsovaoqgm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gxbcnnthj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gdwibtatu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gjoqphjgy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gpkgnrmdl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gxfizvnri.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gkdbessrv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gocwgbume.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/geyneubpd.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gmxxyojvj.sHtML


<!-- 参考信息 -->