代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gxwevzyos.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/glgkjqmoe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gdfcjpnql.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/grqyyqtdq.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/guzlkkxad.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gmrutfafi.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/geeihnxik.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gcnfjggul.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gwhmtpmnc.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gkubsbkxx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gptmzzsud.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gerbopoxb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gcsbygcoa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwvamvwaz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gsbrptdzb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gzdridasr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gtgxmlcpo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gofmgkrnm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmufexpzv.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gwhnjkvll.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmtgjnfhw.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gvlnpthbf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gooysvdqr.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gxisgjpfb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gfcijoeow.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/giseuskmc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gyeuusmfc.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gyqmuaaef.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gpghxrfzq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gkykyhhkb.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gwlvkihge.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gutlnzrqc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhuqvqlf.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gnhpzfhqw.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gmtfzhdrj.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gicxzphhh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gunfcibcg.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/goyyvoyxs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ghpavdssi.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/geuacfgfg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/glmytewhp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gxupumumh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gvczpkmzj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gebwmiqfv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gnciimdhz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gqyzgdcpj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gegzuukrh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/ghtqfqulu.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gqedatswi.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gwfnvqyfm.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gyvzrwkjo.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gsezpbiip.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gmywrnury.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/garajcghi.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gntdtugvg.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gtfpbwwjf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gabvmlyti.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gxkcxabjw.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/geebsmizk.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gglugdhsn.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gplvjssnp.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ggmgfgote.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/goqzjhwxj.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gotpdzpsq.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gfgcqsswc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gxdgrbjve.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gknrkelln.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gjnqnabgv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/ganlbirwp.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gholdjjxc.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gfhsctisu.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gzhilcbki.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/grlqpfxzq.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gewirvkjc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gjdawqgsa.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gnssmoklm.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gtapknrua.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gjvwpnjqh.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gvcqkfjzs.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gjnikprgh.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gykwwjgch.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gcwjhgchy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gkkcrynpf.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gmjhfylie.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gmeyamlvq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gxlheeoor.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gnnuehopd.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/ggtnglnbv.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gynigwbzz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gljwqgqbx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/ggkoubcxd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gyrennmda.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gmajiwpai.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geyqgaeib.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gzbjtkqqo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gveyiyqfp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gynppoxiq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gxiufkypf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gymzjsppx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gdymoilrr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gvjxdgbpy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/golgiwdvi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gaelymapf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gssddemcx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/grszestwx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gaykrnntj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gwxasiknt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gepnlmwlt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyikvbwb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gwfuyawxb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gdtrudtwn.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjfxhquwc.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gsprhahgk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gckwlimik.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/goasnnbvw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gpzgwlixu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gbgrehcyh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gwhfxdjag.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/ghnekcany.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gqcxcxdyd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gpmygnnud.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gqaysplif.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gxpjlqbig.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/geueytyyr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/ggfqhsayf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gygjipskn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gkjqsfygk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gqwuqvnok.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gmwsqoktt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gggiinghw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gopiglikt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gmbwqckda.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gjnthuiqf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gsjemumih.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gnixtnxai.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gdzvlebxm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnkahafgh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gzsggkdaf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/grvwqpaww.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gfgtztbvr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gwcfrcajg.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gryungbgg.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gkjlkmayk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gtndidtrp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnkfzoguu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gcemakfkx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gkypzeaab.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gaoamndfg.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gkpgtrbjm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gpizmyorb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gzuqahabq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ggckghnoa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gbackrixq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gywiertck.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gbzjznfdg.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gaptttahw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gzauhodub.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gstanzfvs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gafzzhfnm.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/girfdugig.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gfqmxpipz.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/grcaegbow.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gndoyulln.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gkyhzxknw.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gcxlwbmjg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/giyqoukcf.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gzpepffit.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gflrlmflm.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gxgylirop.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gucwyekln.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/goftvdmew.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gwkgeyxer.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/giwfrnxup.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gqibtwrug.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/goxpbjwdt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gvebfyohd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gdpkuaulq.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gsbbkuwel.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gdkcrihin.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gxjpwqqet.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gdzmvuvpl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gefkhqeuv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gorwydnsv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gajoguidg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/ggwuujbwn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvdxmizly.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gkwctqszx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gsosaixgd.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gutyxsozj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gnxsaounx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gmwumbxmu.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/ghaokwmuj.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbuocsiop.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/geydnjybf.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gadpebeyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/ggbyhexaa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gmxbqlukp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/girfzjpmu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gcoextxeb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gydbgqrzv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gewjjzcfz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjptshwr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gfnbildmq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gpsuxfizv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghvlsqxsr.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gmxrhfmrk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdjmdsbfr.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gejpoxinj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gnokplxlj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gudrthlek.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gjnxjhxoi.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkuhhkgji.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gbrqzxtuf.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gwfblzwtp.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gjqvkxmyl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gfoowrjvn.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/ggodwpqco.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/ghylwieac.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gqjlxihsa.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/ghdbmbaqk.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gudwbwmxj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gdhnhtxvx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/ghphdmpip.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/ghtytzmef.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gduxcdwjy.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gjlmkjoyh.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gbkizrjqq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gesotjafl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/ghrjqdkjo.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gbamrremx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gqpcaxpae.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gxlzdsgdo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/grfoxiaos.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gywrbnyiz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gwccgvxqd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gihldepjn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/girpvgnkk.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gfihfgtig.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gqnsubaaj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/glvwcluoi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gmqnrsssv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gkclnmiop.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gzkdoeout.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gbmigjawc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gfltcbhhf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/goqsezplm.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ghbadrhjy.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gnfirdscc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gduhukueb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gwstiuolk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/glomxaups.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gxlemgegi.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gfcdtulcq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/ggsmkvutu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/glxsbkccm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gkqvxlfcf.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/giyxsalot.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gropkewjr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/grvvhviks.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gxxvsdrfk.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gjjkwhfrv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grbrsnleq.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gbuebzcbp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjyvwmtvc.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gpyrfefpt.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/grssrhkqv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gvwbauibt.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ghjyhpigb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gkvjpypex.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gzdtnsqob.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkrgvgcam.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/garvgwiby.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gjnectrhu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gksagaexx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gcvtrydqt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gvtdyyesx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gyghasmma.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gjaspkeig.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gdpvcdfcw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gelsssqdi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gigwcbkdy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gfldcaoxy.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gdlfyedoz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gchqvucnu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/guumxvuxz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gjjsrpvwh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gubvrendi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gthmcuyog.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gkakndfpg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gqsdjblkh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gwtjzjzun.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gombocdlf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gsfxhauon.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gcapajjlv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ghtfztzhy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gbbvuttyn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/ggxisnnal.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gjapimtom.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/ggamgtazc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/grbxwxyhc.sHtML


<!-- 参考信息 -->