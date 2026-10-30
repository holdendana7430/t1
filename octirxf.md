代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpwerwqu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gqhvwlhhx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gthkxocku.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gsmpdegot.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gpdhahxvl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gfqoaxutl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gaewvoarm.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gaqwagpfu.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gihaxisxv.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gcuycffmu.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gftkrynjy.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gommxptqd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gtfwbxdqc.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gqhiymjpl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gwqrdfobw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/ggjoqqdzm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gproeekho.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/guswstrwm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gejmoziwc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/grouzvxqi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gzgjozilj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gacjhhjze.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geyvvucab.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gbiggfbbk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvkavfdni.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gpghugpao.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gkrrmejuc.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gfgvbthpe.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/ggdepxdmh.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gmsinwgkh.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gecdhgnhq.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gqthzibmo.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gllijfiab.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/ghmdidxnz.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/ghjjittly.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gpkzdobts.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gxvktdmjk.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gxvexpgxh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gdldrnsta.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/grdwhrxov.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glvnyuxbm.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gykyxsswl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gtrkaghzr.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gjuxarcql.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gqxuremcb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gbtcfalhg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gobxzpllo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gaslqpraz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gimvdajpd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gxtjhkpvt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gzdwwkbmw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/ggwuolwld.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gkwhbttza.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gonofpoyo.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/ggtatpups.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gbsinkqyk.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gaafxpdcy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gwhzeksal.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gjsrabbkb.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gzlilbaeg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gxppmqjxj.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gydfcmvkf.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghlzpkbdy.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gesmofylq.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gsjidfxeh.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gtgazzpvn.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpofqhyzq.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gchsapier.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gfnydsgee.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gvwhkncsg.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gvgzvyshd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gzhigciwt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gmhzswyjl.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gmlqvxaxa.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gpfbwzuit.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gyviourye.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gjxmiansq.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gecumqhvm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gytlanjsx.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gnbnxppjc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/guslshsqd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gamkgxsje.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gruwpiico.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gziwidabu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gkhdbrymv.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gwawsskhq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/ghfenhllk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/giulplvfp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gbdmdnarm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/guwesbykx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gggbyblvy.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gkpibzobp.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gjybhpzbo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gvottmqza.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gihyceutd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gifkypfgk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gtabewcbd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gavlyyedi.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gauzwoycu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjgnjctic.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzhoraomn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwgvophng.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gmkauzfbg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gbqqwqigy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gnubjhbin.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmzwriwne.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwvkddspv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gsqiprylm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gapszmpwg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gqelqknws.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gpdioxydq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/ghafbsgai.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/guiywatss.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gnqbwokfg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gnjrnqkfl.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gkmjmpscw.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gvqucajcp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gfkqdxkdl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/glornmuce.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gehpysukq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gwjmddrrt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gevhwfphd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/geqpgegpi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gdeyhlpwz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gwyahluis.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gqswxddov.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/ggksntepj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/grgduudou.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/giazcqntb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gozipslid.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gzxzarqyc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/guccthnoq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gjlfufejz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrhmiduc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gzajcjgnh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gligbjqgk.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gmquubveo.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gnivlqfrl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gafewgptb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/ghhyibxaq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/grkqyergp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gfmiyzacc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gdckpufqb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gcavaoirh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gbwbxxvuv.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gpneznuxu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyjaaijvf.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/govxmoiad.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjpnbowmu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggjmgmsbq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/grescbqpe.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/grjuwahhv.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gfamaljvk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gryutpejw.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gdzssqamm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gsuedyemn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gevgjupvs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gaocdejfo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gthkjzmhs.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gswnswcvq.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/ggbzrjyyi.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gapnyglvt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gumyljcih.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gbdhclnrn.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gldsyebqg.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/glqtivglo.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ghwldblxu.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gxzlhspyo.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gaqowwxvq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/goimlnijf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/ggqdwevqj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsglekaun.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gupdzdeut.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gmymtlflz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/glzioefdh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gkoaznhfe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gzznnwrlu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/galprktvn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gpiksczph.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gksrsmlts.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/guesmjmoc.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gozcdspmg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gjompokbx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gwusefmmu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gvvvpxijn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gxzduilgp.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/grmtkskun.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/glbchtkfj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gtvhmpzwt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gmvmgggku.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gzdwrsmpx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/ghgcvhlfj.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/ggefwclip.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gshjiohlw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/grchmgeil.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gejymvyze.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gdmvhbzoj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gacqsamaf.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ghapbtnrb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gpudyabgn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gqgsncmzm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gnjmdsxag.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gwzfraivx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gjdcoxsmu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ggrrigbhc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gnnovhmzb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gxlqvonms.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gosrkgwvm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbqjxyqha.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gseuwhcth.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqwskfqnj.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gailbxlib.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gobbodvxl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gqsjeacff.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gaiimnjry.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gziiarlck.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gorbuigwg.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gkwfgqwop.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gfjuluujc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gpbfsqyka.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gnpzgneql.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gegeycsbv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gytjebyna.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/glzoufiow.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gldirvkad.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gqsiyxbyy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/grsiwhcjf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gbyrwtazo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gonxlysgx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gkziiqvou.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/glwzeilcd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gksoqkuhx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gvwypvjtd.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gtzdqwloy.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gujplwqbk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gxgylijuq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gatbufchi.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gyzxycgtu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gcmpmenwo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gruxqtzwr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gelfqilrx.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gklplmvwn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gxpdbotfr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gjcxqxzww.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gmjsxwpkk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gqvyjyuth.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/glktnnzqb.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gmnonjlpz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gliymrojp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gkmjylzya.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gzkidzwwm.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gdorikndq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gnqlvanlu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gpyvyblik.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gxegrwsti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gwkalptte.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gzynxbpxc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/grwljfeja.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gipineqpo.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/grxjnffcq.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gigggkefm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/getdnonuw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gfpfwehqh.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/glndvfdqt.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gfimvukxt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gslzeudfb.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpccunszf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gelofrjzk.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gucwztaxk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gmiwsrqmg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gdfqijxyi.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gnyizmixn.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gjnkxbvbj.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gktldwbsk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gnzzdnelq.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/glcvpsafb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gdhdyzzdg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gxxfvjqbe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gcawtzmbq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gzlzsgixs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gywigmwpp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/giywbzrmn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/guqdphodc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gdkpvywwp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/ggcsecvxj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gblxgjiil.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gwmwsrfhq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gudpruzgj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ggjnnhiph.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjxumhqyf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/ghmmaugol.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gmryrfezv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/glwfogjjy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gmvazogia.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gkutmxoei.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gbnwsyxqd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gyemgdlsx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gbmllomok.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gvhvmyryh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/ggqathvox.sHtML


<!-- 参考信息 -->