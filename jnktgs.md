代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3iqskqndr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kxanllfl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qqhvoluh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ygtalotu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hvlpermw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ouvgxgte.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3pdrwcqxi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yaxmugxn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lfqsrsoz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3imjazgci.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cyxgbmfm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ohicfuqc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nckesfgg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lpcgucca.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3yrmkkivf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qeixzkzz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ybcmxafl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3btuqchrh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3aubxrklq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ltxpdpbn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wbqfnmcs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aytcvoym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbmtiyqr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hxybyrsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdtogxlg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ckokksae.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3dsujbxix.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3unpnluqs.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3psmpkhkj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptcicgzf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kdiizbtz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mhnkvqry.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jdlhfiif.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fohkjjej.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3skvknicv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mrkuvxdp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qopiesyr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jvefsavo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xgxgxkds.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vqirehkk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3boryoonc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3lcyxydlq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bdhmpxcq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vnwuhfqs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bhwpexft.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3tvzzlzzc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3izcdvguk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3etnuwcjv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3urttnion.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3csllobqq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hysuccpq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fdwxishu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3szqkogro.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gfkhxzvg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qfkszmds.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3luebnbqx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ziwuvobt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bnetcrct.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vfhhvycj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kzqxqmon.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cusrgqur.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cfgsjnfq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmbgtsiv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cbocfvgq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cleqtkyc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3srivueyu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqtyzsk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwtdyptp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfyomavw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bljotufe.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tcpsqbzy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wvlbesdg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iggxwwtk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ubptkfsd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wiitrypu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3izaucktd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kynppxua.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tfypdkpc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yvohxgeh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3afhvfeoz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pwkrdtbs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wvhcbhfy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yweorcpf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3muucgewo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ahbuxclf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3epkrazoq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3swvnbvum.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wvqlehax.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mhoqblxb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xntcaltj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ofginaup.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oaojjhly.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xhutbuxm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jcpysfdu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ruezeafj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gaxsqgfx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zmekkgvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etdnvlaq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hwlobiiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jajnavgd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xfsjokky.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qrrfrltc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gbyyldcc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zxyvnxbs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rmjzcnaa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3trzmlogv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rejlgqdg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3eivjearj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdcxonzs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ieiuahny.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ywwggrvk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vhwelqoo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3roipzcsi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rstelwqp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3toafegto.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qurefrzx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gyvblfkr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fxknfgni.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wmyugrkm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rowdjngc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ltpsagnx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fystnevf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3inhztmlt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ktpytddf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cyyfdzxi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kzyxdcqf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zzrylojy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bmmmgnki.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gaarvmch.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3asjzdvkw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rawewzvz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ygknzkyd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcfbucne.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ewlvihke.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eoohuyou.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fppzfvkv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dahxcgsy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fssnoovy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvrhcvvq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3enuavnwq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtvsolvm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pslybwxc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qgqjogog.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tbzgmjnf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxuyhvdw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3meurjbui.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3etzttklf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qxmbvjjm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3klpykyuq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3radhakue.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qyjzywri.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3reviuqjz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jlqkpugc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dlpojzam.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3wbevwpeo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3okbrsgha.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rcpmzukt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ccqlmrvb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hdnzcmsb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jzxldpui.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cmbpvfuf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lbwujxxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jvjmygus.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3phbjbvno.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jtatqwnf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kwworvcs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lwxoislf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dpxvyytx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vbqvhezl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wsxyqzsn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kslrwjny.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mebbgvjn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3svbodfvz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jkmqictm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kpzpxhue.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aiayvjek.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xwipkoeg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ozrmimoe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ywbaufkd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wftlurnw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fvlnhznb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hcxuluvx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jbgjdnnt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nxcylhxx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lglgbqyp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ckbdwcde.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdjokdwc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3juakkkxf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wufomudk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3eixwbmmu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gxsoluva.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ovdsupyq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xhfadukw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3yqzzmnyy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uwsiyqbn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ytrlgmnw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kuvbrmkr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xhjkaouu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dqbdzmyh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nyvkndjk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pyvljhoy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ovtnpsol.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zwwzaqcl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kspcrgeo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3osgojlpc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yblomcaj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pyhhfbwm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3voajvvgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwndoskl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3trnqipfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuksftpz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xocgsnag.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3tnsbhdpz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ywewfqlr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3apkvdwxx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3luptgpel.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fwhqxpql.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dfengrnc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qsdszzwl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nzpbyzdm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3piopxwht.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ckqvdbvx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zpxbyqci.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dubpsvcc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ldlectol.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eypmkmgi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ktjrftta.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ytlprbbh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ppwetspk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3svbgcrgk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wiqkbkep.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3otxbmtkp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pakplfuv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lhpljkii.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yomqlpqg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tmyorbpt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3chazctay.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyvlvjyu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cyzmakva.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xydhqqre.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vnmigjxo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqmdccfu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3thfjppxl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lffbvwwd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3vnzhwrsi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3kafnnlll.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghelmvjz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bwpujtpy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ytjyksye.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ighlauzl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wpkfzzyx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ifmournv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ycmlxtso.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dfdtdbie.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dhlodqsd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3recukpwn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3bblvdsyt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3yslqunzm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vkfmevtj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lymprshl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iurvalym.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dmewtobs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3sbkcrrvj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jyzqghmn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nqbpresb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyfuxoeh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hgwlhbbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwobboyz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kqcvwddw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3pnnmdbxy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3usnceipy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yxlksxws.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sibcahfq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lvtigcdh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3sjjguqvr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qyezqmej.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gzwtypns.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qgvzlszx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ioskljsx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3shavbrah.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bmaikjbx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3npshuheg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dgwmpidf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3iepckefi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thekrclb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3rmvxjmdk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eaipnpss.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hdspdqsf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3qtxmjikg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ewipmdis.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jslnkqzv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxjklgg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3legriuox.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ukabiakv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kcwahqdg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nnmqqeci.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ckddybsv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3amyqhgxs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3izecoxwh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rkjjjwji.html


<!-- 参考信息 -->