代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yknzfbbh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bbvtkkwi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3geqofujh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iqwblcjl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gqswotkx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ipyqkrzn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hmtathxb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3bmbbnvwt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pqfvbcrp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3olbivacc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3utznzuqc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mejfumdi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cbvidzbk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wcnrzhgb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3akcugjay.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rolcflhd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tvemfpmx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rczdgfea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgytroyy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ylgtcsbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofplncir.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kwsbgded.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tjubdgxo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jssecexh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tfqxgxwq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vccqoovg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sawexlwf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fodcpzts.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mjtkwgej.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xszqlwuf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dcrvpxqw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3usakdgde.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jxlilevo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rrxtmvci.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3riyoorkv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nnzlhzid.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3prwumpzy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3komkvdkh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lzuovyfe.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vcsybmms.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cqjrarie.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fqutwiyq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xtkxqhvw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fskvrizb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wbwzrnkv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dhlrcmqm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hhrurqco.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3oantxwxq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gqhdnalo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zhnkoigv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sahmaegj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tszqwlkh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rwzzprqp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fzmgoqmx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ssrcmdzq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xvrdyzme.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ttyzptyp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wvhzhmwy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjtuxlok.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ptlcpgrd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrbyomo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bajfhqsj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gmkshftr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jkfkkbci.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kshtbfld.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3uihrqhcc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qumwdjmo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tkyhprpv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vjailhgd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kfoygbrr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fwebfikq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3caqpfcxa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xvjefbom.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3myrirsdo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yrsnrxbt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wponnsjy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zeqbklgo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3pnauactm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3knuxjmkq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pphermka.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ftebsyhk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3citbigmt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xxbmppfz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vahgcmrb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3nxkkfrdo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zjjhwpyf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ylqiiypt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tzzeelct.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fdnnbnja.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qbrlcxnc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hqifbtmt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3isfcacil.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3doiazuto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhbdopiw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cjjcmifd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhkofwki.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mrtbsidu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jznrafcb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tsarnbkd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tynheyvj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3navbbpqw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pddutzem.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nnjwtnfz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wuykuuve.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtahrgl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rvgujilc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dstyqomp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uxdnflzp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dwakmebd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3usgthgxu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oodfodju.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3emawcgnk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lgeqdcpw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rbdhlptu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3tsxifwxi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vayjbexw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ytnzvnqv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3amctuqqz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wvsgcjay.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wqydoxhj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cfeedygi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3objrpvqv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tngtrplx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wuglqyzu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gexvghjo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vwyolpkk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dhcaywjh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lqpwaotr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rkvhblqi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3egbkrqoo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnduozsh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3trrjfhyt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nfdiilqi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ymsnuhmo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3adlktmlq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxiaimhx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wpmvjnur.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qcbkcblx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mtwdbmnw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vdpxsmwk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqfigrih.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lnvzfwjc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fkjdncsg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3epngizqq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3czvrfkuo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3syyulolg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3msydgcwy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3chuxkoku.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lahqvpip.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ujedbmtx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ggbvgnzc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pojlhgjl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3utnwvlwl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qjusxosc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hunzbjol.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jntesajl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3upkssvyc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ohqcggbo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3uujrutal.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bjexqnsk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjembpk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lehwxjiy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3obyouodd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dzgwglko.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hkjnywwg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tdljubgx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xdhrlhyc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mndzgajg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3admxkujb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3glxdbnzg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3phocjozo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ygorapur.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ugrwitze.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gqweqopu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jnejyscv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ebullzdc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3guvngjjo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3uazwmplx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ylfvwmza.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyncwugt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ufukyqgu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3viarfthx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgiewoex.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lxeihzzf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rackapwx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3yvsdmdxm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3puenqdpl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sohuehwa.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mtrqopku.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jxqcmhen.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pkfynony.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mvrngojp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qjmuortw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gdvlmtzo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3alpdmolj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3uguevrfc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vowtleln.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3olfxirvy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ajbslwpv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ontmbekx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ufdsrtqa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xuiiwitf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nfgjanez.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uaxjtjpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lodcvmxc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mgcrevrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irluhhou.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vekrakhv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tkyliycp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jxgqfrob.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ktnkplxu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vthvzdiu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kkjairdp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3niledupp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ahaydexz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cftzbalh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3eiznwakf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lsvofdwo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3geggdzby.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3grbgjczj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tnxfwurr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fmvwqyen.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mbkoysgv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zonczfed.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3strrkhun.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3thkmauno.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hswxfcls.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3mblxjhxj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nrlerspc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mddyvqzz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zatdggix.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nknzqukg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3afowddsb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ugpgzuwg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dsjwskvl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rccvfhzk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zaloodsc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dqjsmaot.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppwmguva.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bkhqikdi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jxmqbamf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dflzdqnq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chnzmlrw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zgebtsqu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gsboqons.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fkdwgbpx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3sqkgnhlb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3czsojvib.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fsnqgzfv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3szmwdbli.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvocwnt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3uosszjms.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gimyhpdu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kdcnyzen.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3gehwifhp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kewmpimy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pnbimlxp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yzohqgfj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tkusbplc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3amhbaxvp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zxruywcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfabaqiq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dagsrznn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykxmszec.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3agodauna.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ikaupkyy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3keqcmpwb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gufklemq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3feziopvc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zortknll.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uphmqlkd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vlqfzkqp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qpdxmrhn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tlmblxdn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3trcrrgxu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gletmwrk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uoykpepr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rmzrfwer.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bnztxkcs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dnbpvjkx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bptkojlu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wutrignp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cbgjvttw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qrocmtjq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mexemcew.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wzzktisn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bazfnvdo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uxnrlykp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3umlpsrjp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zlrvhkzc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uskrzgmt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3wpixxxrt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3aruogiqq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qvgwuoyh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3khxhlndq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xgpgnvzf.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ownejhls.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuqcjyo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3liyymauo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3erkqrjff.html


<!-- 参考信息 -->