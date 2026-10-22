代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwgevxg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2uzbcvlke.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2bdbpqion.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xhfhlygq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gzsmnsne.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dpkzmlyv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2foydozyf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qpjuplpl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lfgiemzc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2pkxahifa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ohjurzxt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rryvzcvi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bvmfnhpn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nyhpdfqf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mvfvgeor.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jkfpgqns.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mlhrwsje.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dpjwseog.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nhxtroeh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2nzgiflgt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2myfpymfi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nkypsyfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdynbetz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jlqbuixj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgltvgkx.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ywmyshre.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cyijxgxf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xjnybyly.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwlgrqll.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oemonmob.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2johdjoga.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rgimucah.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ktfowezh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dbvoaeod.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iklptbox.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oaohkbui.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ffwjhhim.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tcbxsavm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uedudmrx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kpzfodsc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kzdrzxsj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dpryjwaq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2enahnvdw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fqdespfa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gwasegwt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cirkdain.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eewlrvin.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yenvrzuk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2jgqjrpfv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ttldessq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2vzwapirc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jikqcloe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gaowvbzy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2khggwkar.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gsrcsdva.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ywrtlbsw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2asfbgsob.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ofnytdzw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vsoxssaj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2iocgyddb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zlfqexia.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2laexqmbh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnfjquav.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2agmcuzsp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aklhcjqt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2midsqdju.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2liahvddk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2owqinqqg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2djzjcdec.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jqyomwpt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uoduczuo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ajlsrjme.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ryilmxls.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kssnlnqb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rsnluxuu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2efdlqcde.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ufduymvb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zpaqecnf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2beppvecv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yironqhs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xmkeotza.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xljpbnks.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2shexegpp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vpwynhtb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2deqtepxl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fsmvvmfq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gucbzkze.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkhbmjd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qvnfqpiz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2yvbwznmp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2egheowyv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2icigmcuc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2udqfkhml.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2yctngzqn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2upzrvcmz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2camhvlrv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qegakfxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwmahman.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xlezanyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uigfjpbj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wyxhhzrm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gvmndaes.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wydfcwwl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qiwznitf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fcpwwsxl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrtqzgn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pqrbimoz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2euuizufy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipjlwalr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bswaqmmj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ohcikwhk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kxoneuzo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hhyjxrsd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lnnayfga.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2fnjyxfbl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2epsavihz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ejifapsy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kfgwibuq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rniyiwlp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2giexyrkw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2poatukjs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ajhpuydh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pfupzwza.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rtejrrjf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jhfbzdpk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2teoqmcbe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2imcctodf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ubtfazzw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgegpacl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxxaiqta.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fbkisytr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ivyyvwqc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtgpiffp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2labrcojz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nksmlcnl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ggauurjy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qbgfveol.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nythnfbs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uuwvwofm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxjudwxu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwrwbicx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ucqwagts.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2apdmeept.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fhhafehc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lguvbkmz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcgebshi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zvlolieh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qzyopeie.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bnwuqsuv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sgiwlsja.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oezarzge.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2etczjjct.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iedmuwli.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sbjcmarx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hqtcflco.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jktpyuph.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cnuiwpxx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wtjvqydn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nqsvraea.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2majblzgo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kzzgyjnh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ufbinsxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xliigamm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzgqrc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdqiziva.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2igqioilj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qwqxnkxw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eqvlockl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kmophdob.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uyadbtyk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tvlkqhxw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oyzlbplx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hgxnzibh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dytxqxtx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rhtsabbg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ocuabtlq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rqiwwcdd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ygadphkb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wziyzbep.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ndrgoerb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lmapfgth.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yjkeejyr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nyrncxqr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lashuist.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cosgjtbq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ekrrrsjy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2arsunuac.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2taovzfyv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2lnkfatif.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rrwiigsd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yfhjvtpw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hxcdzkbb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qfglcrew.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2srsmdajq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cqyvdojn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ojqxheqp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qsjriwtk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ocgagbcw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rsmlzvah.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xxboucwy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mdsqteqs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mahptred.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cjxdmuqa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mzwjcqmw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fgnhbyun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eilfvxah.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oxzjbyxi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ydyptbbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oebrhjxl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ctlqasng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2poxvzgjf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hhdxarxw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2njfrnvbg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2chpaylsl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2zzovkudo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ofccgmuo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ddnsrqan.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wznbxrrv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lbxsmlaf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2knyrssbo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2umalnkdt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xoptynbh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cnwpakcz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2efqgdhqt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ihxmquns.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxftdyj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ezxoxqbh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2aejpxaga.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xohxhehe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mqsirwpz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2drgjwvdj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2nfuiydmb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wonmjdhe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2anenzljf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzuljudu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2rjjntcul.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dlzkdwij.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fafqqwyj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zhpdcphl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gfltavob.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jghukotp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2atlrflie.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwskquuz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2pfkddtzw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xkhdsiid.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fznenlzy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2oxstdopc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2waxjhpux.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tcugfxur.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2parfvwta.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lfikcyfx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xosoqewn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mhfyzreq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2kiljqfhj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bnkqrlyc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vhmahgzl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pxtyfiyw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2opniswkr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2vyqqnedo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kmjhyfbd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yspqswar.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fvlfkexk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qedmxhyr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2oxdjystq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ayfcjvrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikkgigre.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qyabuxce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbxgbytl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lcsiyjoe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2giahkyjr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dgzisffb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mpfeufir.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hpxhmixx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xokysbke.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2agxyrarl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2atiftbsi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cpzolslf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gbllwbml.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fbwbdatn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kzotkehd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zjjvajhx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pyinfhcj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bwpjogul.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qiomhwnq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vcyjmgqy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pbjmnteo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fmecclaj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pmeakwhi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vndnjnsg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpvnvnw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wftregzs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kuwzgqlx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ebtitjgl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nhuhuusq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zwfxyahx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nvzbfpje.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2njznvlvo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lrqlenoq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oscvnlmb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xijyjvxk.html


<!-- 参考信息 -->