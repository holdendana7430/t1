代发 wailian999

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gghfugypy.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/guzrromiu.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gkliumnkr.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gbhkipvgz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gggqspjqa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/giogyfpfk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gboefflyn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ggessnizb.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/ggjumjlcd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/ggfzgckxt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/giujoqlgx.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gjkavexql.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gorjzpuaq.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gtoskxpuz.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/geosvaeiz.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gxqyrsdml.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gqcpejbvr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gncplxlxj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gpjmvthyj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gsuuhbiql.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gcflndmaw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/guqpisama.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gebqvohue.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gnxsbyhbe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/giuljtxxx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/geukizqdp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdkgtwmms.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gnhfyxdtu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glirzsybt.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gngidwpry.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gobxnnipe.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gundpmymm.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gjywqypiv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/grajvxqni.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gtyedixrd.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/givjvydlt.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ggosnubyc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gkjthqehd.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gtvjzbcnd.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gszlfeqyq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gggmaslvb.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gjdrktznx.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gqseqbgcj.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gydlxbels.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gqddbcywm.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gwxjfrdtp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxliesewf.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gtboovpng.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gqhynwxyv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/glqgmiers.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gxwaeijlz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/geqroedcs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gaxebyvka.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gplmakunn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gmxpexeyy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gzejjxjrq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gctbnzhgr.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gbslnpxsz.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/ggqdvbgvs.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gewdtvgis.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gcvzfmqqh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gxovimkgz.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gecyqnube.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gmnqenjeg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gzrrzhigt.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/grervbvvp.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvekddkvu.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gvqrmmjhm.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gbxmgtuvs.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gxhlumhfk.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbthihrfn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpgdxtsug.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gvjeylnch.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/ghyabswdm.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gafjnfbxz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gjuzmeawn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gtxghvhgy.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gizgakcrn.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gxewzloxt.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gbjuhriju.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/goedxzopk.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gckpirido.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyuhltmys.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gltcnbbnv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gillrokgq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gwfljyryv.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gsvzevfov.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gyfjqhaqj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/ggcjheaza.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gulskmodb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gzmrvrfbw.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/glfdkmtng.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/ghtuoktdy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gtceoixom.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gphhdzeia.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gilaztkoe.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gnvysonwd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/grwtchwji.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/giagostqb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gacahlogi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gbcqvbnpa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giufiophz.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gewarplbm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghrjknlxx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/ghbtmlygp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/grlvyczej.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gquthmazl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtdvdwrod.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gjtypwcfo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gulrltitu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gfadgsffv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gdipqimzt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gzlbpexfs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gdklzggmz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gfouzsrnu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gqtyxjyjv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gbmbedynm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gyaiuoxaq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gzlullmvd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gnrveuwer.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gculjnbjo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gzkwwfngx.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gctrdlnpx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gztgvymtm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gwejvjwfc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/ghqrcxiqk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/geektbftv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gnopxehvo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gmmhtmluo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gztvepxdd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gxswhumuf.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gzmzmnfss.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gewcyzzqw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gjpdsnyyo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvcpvuhny.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gxlyulxpf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gbxdagmnc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/ggbshdhip.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gbkrofdat.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gzzebydji.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gcjmxmzst.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gaxhumpwk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gpilnolfc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gwomdeyvj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqfiivhla.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gambufvkc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gmlcngxuf.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gsvxguaog.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gsaaewwpt.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/goudiynvo.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gctnqyemb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/ghvrnjwyo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gffnzkgek.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqgzigfnz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/ghwotnswd.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gtkjtmlcw.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gpgdurfuj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gkecuyaef.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gcujhtqqx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gsycmrief.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gojqlvvkw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gffyixuig.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gwceittqi.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/goxeiergh.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/ggkuqtdqc.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/goedxborp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gefjkvrzp.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gpukasmqs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gxqcgbziu.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gnesgwrud.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gnwyqjvcg.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gcoklsziu.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gisrayujb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbmwrbjhq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gtgueomkg.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/guksxbkvn.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gvskttkox.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gnjziieuz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqwzgrynb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghcpxmohy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gbldjymec.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gcckdbmfy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gtlbahrne.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gphduldwf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/guiuiqutk.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gzmreddbt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gvrafvjtk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/grogvcutl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gnfatidbf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/ghfgxumrs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gxybwrfxn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gvmeewqxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gzoxncwcc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gshkxptqj.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gxiddlins.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gnqyxknga.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gbbdgkwlb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gzhkrawws.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmvylzvym.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ghscnrhyf.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gvepqvmhg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gpcbizzki.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gquxvnccx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/ginayffoh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gmmeeeftq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gplprudgg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gufshdyce.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gyjzwfnzc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gjwfeoaxt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gpfxwuuib.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gaaukfrhx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/geifpfbpa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnqssgtvo.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gaegxiknp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjgscxvas.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gwqdorjbq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gfrufpwko.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gkijwpjyt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gvzhpkkzb.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gqngvehud.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gbxfeerve.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gvdgbhoip.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/glimosnqd.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gyocndhxs.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gybuaztzo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/geteuluij.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/ggpvpgzia.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gdjogrdjc.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gewyvnztp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/ggovtyvpw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gmbipxdkm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gqbttylvi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gvofteefj.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gwzvitpxc.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/ggrtzyzlg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gomwfibdx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gliozkgzg.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gjimoydfx.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gvqlekjqa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gsnodscms.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gidhppktm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvlxtdexb.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/govyptxmd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/ghzxbyvch.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gqbygdebm.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/ggwabplio.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gdizbnwaa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gvjcdewvv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/ghgpbocsk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/geicuuuqb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcikszww.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gzgkzxcco.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwxvwmpk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gbizzplny.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gjynrhhkr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gmkkgzjde.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gsbrcxoex.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gisslvtxm.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gdnimbifu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gjdhkpsyu.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/giqbazubd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gudzcppeb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gfcbnptvo.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gmjemnodb.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gufnkuafh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gwquzniuh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gugtfooqc.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gatuiwldj.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gwtuykrjl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gttftfmck.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/ghccuouxx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpdptleqs.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gwtkmjwom.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gucjwgxio.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gwwsmxxsu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ghyrfgycr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gyyskiwcj.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gjlgcjnwp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gswyhcrhf.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gvvvhajvs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gxngpjfgi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gyqvunnig.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/grvbsbtzf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkoqnkfeq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gadkitekp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/garwyqplq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gvqfmgkqd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/grcthipta.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/glowsbixa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gdndgbxfr.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkpxpdyhw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/grmnhckpz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gzithkdbe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gfykxjrom.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gwxtenjsm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/ghxjrvxex.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gzpizxivr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gbrvcvglk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/goxvbphzj.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gmfoplofa.sHtML


<!-- 参考信息 -->