代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gnfnvfqll.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gvfosuomo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gdjaxagsw.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gmjeeatxu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gexvardry.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gnlforsqx.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gxrfpunzm.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/giilawfje.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/ghbzsohak.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gkkumppro.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gqgofxkif.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gructxklh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/goprrwafz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwfbpnvrk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gzmjrxykw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gtbnhshpx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gdgjvlvsp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gctlmzekt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gizpwmoed.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gusiiqvyn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbseojgag.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/ghjxynehq.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gkkbbawfp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gnfzfjxav.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gheuzxuxm.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gtbydmlgp.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gpmvfqqwb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gmrhypbhe.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/goedhnozb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gmwzilynz.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gdfhnxpnq.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/guikgieff.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gjokhabcf.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/grvjoxwxb.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/ggsccnjam.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/grhpmpcgx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzyryrzkk.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gkmkapxdu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gfsegrbli.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gvwjecitn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gugtidgfv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gpvwkevfw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gjhzytzaf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmynjsduf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/ghpoghnxh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gzggbwjmz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gxghwuhvu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gjotvwqux.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gxxsmvgvy.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gastmstpo.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gawzheapl.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/guaxxmasb.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/giotkrevw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gvipxstfc.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gbkikdwdm.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/genumfitd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/goamwotqe.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gjkxdcsya.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdyrvymtl.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gtmoshwcl.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnbgzbzoz.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gfrcchmnc.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gyvkcmqiu.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/girniwclb.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gdknsqwpc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gxwewssiu.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gqcrbweoc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gqyywuxkx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gfigzsrdp.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gapfozmex.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/goqorfckh.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gcnwaplbn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gjnzxmrrc.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/ghzvuzlun.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gwljcfdnl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gfqvjmlkc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gabixiefi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gbnuhlpft.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwurypiyg.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/ggtnsymas.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gaexrrhvw.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gfzwqtrsa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gjppadbso.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/grjowipfr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gwpkdxjyz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gdewmners.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gwjcdsery.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/grfoporss.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/guitxqhtg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gylyqqvvb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gsutxwqea.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gaqxmeeja.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gfeejwuog.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpvlaizix.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gfxnmpwgy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmtjemlbl.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gcmbuknrx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gabhcrtpb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gcsinhgsk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gitmoaxoe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gzsexwekn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyznfregt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfxgzvhrb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/glwcgzpel.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggjdbwqgp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gtmpyszml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gvkwcvrox.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gpqptafdy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/ggnmancsd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gkbuctmge.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gpmtvlssy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnfgsyljy.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gyvikqszq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gnxkdappz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gkniisuoe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gulkuoalr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gyxckrmwq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gkthgltuu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/ghhxbhcep.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/guqlftegm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gbbomtggu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/glgkuoaxo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gjbatokqc.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gfyzijuql.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ghrtesael.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsyovhuhm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gcbdtjwkr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gnysawfvh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gekxntquy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gkstpzbee.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/geprerwgi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gulccrjxp.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gagprbnzx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gaxkrajku.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gedyogazt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gmoqpaklf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gasautkrc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gzufxlogt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gguympczo.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gljqgucuj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gtfnhzdjz.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/guufevqsx.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gwfrkvczw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gjulyvvfj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/grnkyihms.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxxifzhud.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/ghnfqacef.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gfejhyozw.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gftwuvwsr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gwmvnqkgw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gcauycmcu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gtkkjdocj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/ggsarjejm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gymvxewuh.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gxgeddypy.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/ginwsrukq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/goghjgizx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/guaylnxac.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/geostkqai.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/guagkyejp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghqazsjxn.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gevqucwsl.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/galhfjsqf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gldxfsiea.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gppmalaoy.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpgxvxjtw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/glkmxvbmg.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gvbvnynit.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gszvhewfw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/guovekjqo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/geakdwrkm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gmkqyyyyc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gsrjcgzpf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gqvlhnphe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gmugyueoq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gdgmjnaak.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/grqhpmhvl.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/ggjugvvjg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gpmrlpjnn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/ggohveuee.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gyejoluhl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gygnrvrtl.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gnoqenrle.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlalzrwe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gvgjxlrte.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gzxjqchhu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gfkbnsewt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/geyvwojwo.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gqpumimqq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/guhkwkecp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gpkxbafqu.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gshuuzcmm.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gmsxzmcpl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/ggsahjjte.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gzvjpprvl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gmssbzisf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gouvhhqgx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gpwldvvkp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/glrlumbsn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gmiirvamd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gyyrqzvyb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/globvchbh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gzibleown.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gzyyprvpo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghmyvmuvk.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gdmxjuznh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghfiidjyy.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/ggpsdcafq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gywspmeii.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gymslbzrf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/giksitnag.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gsrsxlfko.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/goondizxv.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/glihynyza.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gxmvghbof.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gkclottgc.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gldlxxyub.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/ghqmufotk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gvqmrenjy.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gfucyudhy.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ghrpcordh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvvoctv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gbnjuynzq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gzwbbgzzo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/guphnsyug.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gheuqgdav.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/geqkbhlgb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gvuokimzx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gouihyegp.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gylgnmyfp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqcoimie.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/ghdiwkzlh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gibmyccso.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gnmlhcrau.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/glvnutzyo.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gvvlucsfp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gfxiddgog.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gtfpjkskw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gknilhhef.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gjqvgsmde.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/ggxiidngu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gchsxmjxg.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gfrxxmczc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gmycyajet.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gedgvlujb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gfzmjmeki.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gberdaaor.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gphdcgswh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gmiahykem.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/ghjynwgkz.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gfjivavsi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gvxogenyg.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gvdtwfkve.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gkpaorwpq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/grxygzebz.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gewjldkfc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gypjzvoms.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gobkaqewt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gdaqfbyfv.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gozrizltx.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gcxmxjlcq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvgumaqga.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gfusyjqoa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpjzumnhk.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gmgalkhir.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/grlrajmsu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gnftznomo.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ghqifuote.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gcvftvsto.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gwpsgbtvj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gkkaakkje.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/ghsntulom.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gxfamumyp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gzymqfkkk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gojujexmi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gdrhlwrsy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gqszvlqgc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gjsucztfe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gvlkroesx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gfdgohqpw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gmvjlbkaz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gogsziaip.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gvnzzzqfk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gnqenzfeu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gwhsllllv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gxzsbeknc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/geftjhyju.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gkapzrvdp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gpkpibzmx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gdhtqkosk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gnvzswgvh.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gnlarupxr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gdashwssx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ghrhplnez.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/ghsbgruqp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gkkukbojp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gvdjnlwjf.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/ggbokzdbr.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gcybvrdbp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gubozfchx.sHtML


<!-- 参考信息 -->