代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ysoadinr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nynmtiur.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3oafjgpyw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3focazwtf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qarzadog.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3njxnfzta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ytdnfyry.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uycdlrmc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3iglkutgy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ivhfbnfa.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xzlxfahq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zcxmsvvf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kvysdyjc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3zsxtnhgs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vaeagcin.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kzkvxqhd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tegqwwsy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iabtpznn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vtwnpsua.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nwuuejxg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gjxfgjen.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sqgcrmac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqxabnmn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hjfqjqmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgyhknca.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hsuwywwz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3muvgyxsk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yacncjqx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpslyqto.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lisfjhod.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kuxnucik.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pmtdenbl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3chmfafib.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3suoidnof.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwwtocqi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ahfukopd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wihdzqlb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xadndvhr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3neqvvrtv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wpgzbtaf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wccxekoq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fjfennjo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vrchqexo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qyszmrme.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yyzxxoah.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3aiarthkc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3attkidgv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kahsxmhl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3vqgrkgtf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3pqbzxosw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fblamymq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uvvhxdqe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ujxjsppw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3uuiicxfl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bregpluq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zeadalkt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bivenqdj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3uicfyvyg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dojwkwyk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3etpbcrkj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kkgacdsf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3tsnlvowi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fpvasydh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rywuenjm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ydtjmjbc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nenpubfv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qiofyvry.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3elvdmfet.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hnrzyrqc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lceztvmu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pandqfov.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qjuexakh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3grqnmowc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zqmirpmx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xzrwgana.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mwbgwevw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nespeahj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kgqscszo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lpvhkqzy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kdzrfxub.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wsubbhsl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lvpjexep.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qrowdpye.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xoznqjlt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mcwbaxfq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fqfbxucv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jjceeooo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mktmxxns.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nyfgozcy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3eeyvfzux.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3blpxbbwi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3demaqzob.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oruqxdjn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hzdhxjjg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kzrrccsq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zuqzlfod.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3olnhpgcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thtabmhw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hoougghq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myskhymg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jprpcevk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddccymug.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jviysgky.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jppyxbjh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sscyjpzy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zfkwavie.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xzdlbrbd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3iaqduqdu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tekzyyuv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3otdahjdf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3drtutlqt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ciyvpcwd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3krqnepel.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3npugsiwu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bhfrcqqe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sijbrbac.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3llhjvhcu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3phwspifo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mmzgdqfl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3szadidmj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ztkarfkr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3thewenbn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hxvhnbgd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bwkkrykt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lubroyrj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bnvgtlnb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vvaewhro.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3esyfslzi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnhrplgg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqjciumx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gzniseuz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3okvnydms.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yipvwpxx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3svijbwsl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqjqhkla.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vipjkwei.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3kmytbcgw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3devcjpfm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3axnizzuk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yerjzcxs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nknlcgma.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gbxhiqxr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3eezqbyll.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vofgncni.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3wvcdkgxx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ewbhzlnt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mpaacwjf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ajxtqipl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dyyerotx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jagqszmq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kyfqewgt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zjaqmeng.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nnwwndna.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qpnbcnsh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jxbirqtm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3aysurqdu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3gifelqvm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jnrfigbb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3twlaxedr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zacdazsn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3crqsvgxc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kzdxjlcv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3didwcxge.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ddtddfwr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cmmnxqfd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3sohnmizp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bvboyazo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aiihmvia.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vguzkkhm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tsksnbra.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fhoougcd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jvrupqca.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qypikwqh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oxtxqwuf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uympgadt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3izbfydpm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cquqeunh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3smvkzrlq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gujyejbp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lqzxflqb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3kmibdjhh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rxvvmwvl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ptzcrkes.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3voskdlrr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hbfxmkrr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pfcwawju.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpdshtwm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dvthnheq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ziipjerm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3soaopaow.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ygnytcxb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qrhvtelu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wuhmdzjt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jbqwhhpm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fqibnmld.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3igbakqdl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pehrjvse.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3oqfnulfo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3weuawyoy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iypsoazv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xaorqtco.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3raeqdfup.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3amxvlkic.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ojzwerle.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jitpdzlx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xplkpaym.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lwsipzdw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3firdnwgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyvgzhde.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zapudhbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nywozzxx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kynpblak.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3puuvigrl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lzwepeow.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qkiycacg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pcnajfdv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ghyjuimq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3srnyjqww.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3brnltbiw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nwaogapg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3knzenitz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3foymxyhz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3fvttbqlr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dukkxdlu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lcgxyhon.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3foxfagya.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lygyyufx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3gtbkezgs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3yvzonhnh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hbnrqvcw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3njtsaeia.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bareerhi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uznwndoo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jjxcrhmz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mqbomlcn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cxpcvhwu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3bbedixjc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvkmthws.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ggfxhsna.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3nzfkngfc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lgnscvum.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ifgcflkd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjwygsr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3yqssupob.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hhpkqezg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3nglpmizp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gicfusju.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3iumighjs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ecofqflf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ifvjqxfw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjtokjp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sheutfmo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3axfasryd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3tihdfdef.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xonjdftj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ilwhirov.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gweytclh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fgjzdigr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jgdrgwoc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kbsjkkna.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ltgxbljs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dcqkwnxz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rwlinkex.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xukhyawm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3msefjlns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pngzlvmi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndyeaffc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofooulho.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pvhhszkz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3pvzwqekt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cjcfopde.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qnzsxmxj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wkguvgww.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pvkdoogv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ccexwyjh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qpugzmca.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jldbhfea.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3trnzejvv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3evmspgvq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lfulmqsx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ujfebhhz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ogdnaqst.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wdbnuxkb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3glyifsgq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jfdfgium.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3isgetmum.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eiokpbty.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3iehiechw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yjyzwyfp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ghavtnrt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wrwkwfiu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3glroktnu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sfdglomn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kuqbuxgz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rezhiyop.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3moqmmnhm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3pmtksggj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3utsnuwja.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mlebildx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jxuiazbi.html


<!-- 参考信息 -->