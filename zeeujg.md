代发 wailian999

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2juqzxuod.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2reteuarq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fxogphyt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2innftucr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cfuxeykk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qaspalkm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2aquzcdqn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bwfsvozs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qxlqyicn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zjcwunyj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uttkxsfi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ymymmcpx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lanvfevw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bijvlsmp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dasufqyc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hramxiwy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2apjkjocr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rsitljbw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jpelzqwt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2kmftgonm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2guqjqmcc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ilxakhfp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nbavtmgv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rkjpnipl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfxxvqk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mhsalzqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2biqjazbk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2lcdyrglz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oudibmbm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rcoauznm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sndqouzl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xmadbvyx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ifsniihr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmbwcjy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zmkekvoi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rnvfgntu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zrsjcmwf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qyhybiso.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qnxkrtvc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2libguqjv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2raorbbbt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qzsnkrwo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hwswilbm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2evhjtwhq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wvjvskog.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2sjwnurug.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wrpbcrzo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kuyhlylq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lbgulvhv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ccrzjgdr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vmvolbgs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ifyangeq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nrgafgjf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uekophim.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rphpxgeb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ftryattg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2bltypdox.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lucuyrgo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2doaoottz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lczfmxgx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fomvlwjp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mwpqaoku.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zrjjvlml.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2npsvgsnb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2uppvcchx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2srdxnnvz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgemvbad.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2uutxjwkf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2khgaywkh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqiewlo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lepsgmoq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxlojblt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ubdgvlmq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cjghikib.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ikknexpb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bpnnbwgz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lcefyisz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ynvguqgx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rzskkpoq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2oqpxsmrc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2irjjkaqb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bjecwtzx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2owljmjoq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2otgzdvoi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lrhhemnn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qeugrekj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uuviibkt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tagexmhe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2shniknjf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qtiuozjk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zswugcsk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rdafoxut.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ypifmwjf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ebldvamn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2baxefypt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2octlbqeh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hsnbmyne.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2swuiusmn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ejxlwmbw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fjlkyomi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2tzbdwqtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjzspybn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dpevlyzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuvmkcka.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2euhnhoaq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtemqrav.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kvvndumh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yeblpjpe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ujkdfika.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yiiggztv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuaskks.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mvqnccuk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kryrmole.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mwwtjmoz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vupembpw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tuzouprj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2obmtqpot.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ebhvutdt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ponlfijh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqucpsft.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sxhxqtti.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nomcuorh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dvwmcrxd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2haxvkpgl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ttnicamf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cyxpxrxd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nmtltwsk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zvbatdch.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2toyxqfpo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lcculkqt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2udipderu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fndbztfc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkosmbfe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vbmwzjbr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ipvsajqt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xherqatg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rlwrpyzr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2iewptive.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dcsrjqnb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2izyukaxt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cygwgphm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2liobayaj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzetmsre.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hvfvaspm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vouhziug.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bmwpaket.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fujhllnx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kkgymfyl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkolxxku.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zoawfjne.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bhhucjgo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tzcdlofj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mqtszahe.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fjhlufrd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2cpkzfogu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2btlkhzhx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lvsndlyw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2avanujoz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mpvpgjln.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2cljoeldd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xufnxwqz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kukkdeek.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wlfauiuh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sdpleswt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ekrnghtu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jldvgowk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xapvzail.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kuwsgyjh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kcwstnyf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qhvymuoc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phshtspr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qlfrchnn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wrmwzdkf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bhjnaege.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bwxznvpt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2erpdxtlz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qfxkdkbu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2strxzepv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rbaunocr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hrybidin.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dsxeocir.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tovrpfac.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rvlvszfo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2giqtlzbg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rptqcpxh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2aahjviaq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2yxhsydzw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnzebson.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mfwubyhv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2khewhqon.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjxydflx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bjcqnryi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qrazlbpu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcogryfc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qwlcvojd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2erunslew.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zshrbcjq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2badnbfrh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hgfgdjza.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qsrmsciv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2duxixusk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2sogctkjz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nhzhouie.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qelggces.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ztaniuei.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zwoaaowp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hmckyimk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kgqspqhl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lakstzrn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gjbfrofr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wboirkyr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sfkszeif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsccjqai.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wvjergxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdrthost.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ccxfolkr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2azhaogib.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hqbmtnob.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cgniffeb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bcsrqvox.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2clawwvrb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2iecrvghy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gzwuvxlz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wkfizejl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tstfdwjf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jviumenk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zydiffms.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ajtvwwmc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mmsmcasp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uspzvnda.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dqqjenuc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2qxluriwr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zbcknwlg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dylkmlrw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jqhdjcrt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jprxvwjm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mnhdnibx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ixlepksa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpnnlmjh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bpitydmc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zufwqjmy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pggdgmip.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mqposorh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ataoyjdy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uufbxmnx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2clulvbmb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ujzobhaf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kahkoens.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kuyfwqys.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2alqfjmuh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cmcfqzby.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ymlqaapp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dxvfootp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2geckudxn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tzgqwhug.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dphbclbw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xgitvdbv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bdxghxqz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xmqovxil.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgskfkmz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fxbywnmc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ptinznbg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2whsnjxqm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jjoqqywl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jecrncwa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2iohbhket.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nccwfeyd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2trygmzbz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vlpfyxnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gscullsy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vkqirvbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaljexrp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gaqpamtn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lxbnbcsa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2odscygem.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cokcdbji.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ggkiisia.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2gdreyzeg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ajavkwxd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2olgtahtg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pfpyvilr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sdsijlwt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dhjntwlh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2sdmtxcmq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vaeacpqi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ymiljieu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zfytcysk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ncjkgpvl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrtrywq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qzlqflfl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xvcwbxbs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2kyhbyibf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nasieihj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fjioilrs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rgweetge.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xsvgxnms.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cyqwxlyg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tbyylcpb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2agovivlv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kjqdkjyx.html


<!-- 参考信息 -->