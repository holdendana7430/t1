代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3edudyxoh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rsnqfgot.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sraaykco.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fqcahejf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tzjxqakt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fhjnvnsf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wsvoiakf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3drmewrug.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ezgidolj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xzqfrfmr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dbpurffx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3howcbnkb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mokiwedh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hzyhzvmv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gudhohsz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qoveuisg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xwcbaami.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3igkzecrt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gvbxvzvp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vofzrrhh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3katuzavd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yaxulbei.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3obojhhtf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3imgpbgrj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3soqnegdw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3dtykryqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lomewfpd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lettapjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hulkjrpo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kkufsllt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qbpfdawg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zsqujuwu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3izcbjltg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yddjuvgt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xgsbxltd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uzbcxrjx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3axnweobw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3evkbbtvg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhboyrdp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rwmcocri.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bxodeuve.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tllkrmwr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nexkfoyr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3puedpuwn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ndktyoor.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3lepoddwh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dzepcgqr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pobbyxuu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3efbiswys.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3elfcwmxi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3evsrodcp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3veasudpr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zvyikqgz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zerpttmd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zlkeurdx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ojqdsxxa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cnpqejhu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3weadidsl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ajenphxn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zpzjlurq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tlnijrch.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sukcxvwl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kcnybnss.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3pcrdpxji.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cxyqfjtz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ekgpzhky.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfuuxrlh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qdmuvtmz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhyvviv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydvgmatb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lijrxjkl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgkrdleq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhwqggvg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gpfkuogo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rvlksqdy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gcoqthvn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jcysoude.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qwqzrlny.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hxzrqwje.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wzargtqk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3rgwuojhm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3adrhbneb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gkhfnhjl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kgrezxrs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pazryczx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hneutded.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hvcutrho.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3aodscjhh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jpnjlhdd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rqrakzfo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ghsujfbd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jaihxpfd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xnbedrwn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dwqgrtgb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zglixyor.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dcqqwlqe.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mzzymcru.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rlswkpxu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3itlgpxnc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kuxqljgj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rtkmufna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atauvbuo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3knnopawu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3joorzoyt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3sunlqiyy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chkdrcji.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oopvnjns.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tqsffjjh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rteacslg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lggsasee.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cghscrwe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3grcesyic.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3htwskbdi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zgyawptc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dodjsdsv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zwelswii.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xeloeypg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pyzdvzdd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fecfewoc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3anzunfkd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ixtgsive.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ykbyzdjz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yokunpwz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rqantdxo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qjdbxvzc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3palqsohq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3atdledas.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vnmfrjvh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rofmmtuq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nnqxhjjr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dcshvjof.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qfoynrkj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uuqnybwv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbcxggpy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3frosfwyh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qatislxj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbhjhcrc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3bbgmtkkp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fyoeneat.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nawugkua.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3prcpbgxo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xxeknhpm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3stxhfqos.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3winqhqnv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uhudbsdf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3majlaqwz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3feqvzgym.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xzlcvhls.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ixtzximj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bdqqrxyz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uysiarfc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3srikfvda.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ibuhiujs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3olgydqzc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jxhjheph.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3yrzjjivp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ooiyqace.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qcjhtvva.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xbgtemyt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3weicitxy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rpjqiwwg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mmkilrtb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jjdcdmlg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fdkvijdv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hqbmmlze.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qfwjmfsm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3faqbjtie.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wludmhxt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pclgsfdk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3epdgxphb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ukgoyoip.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3myrozzkk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cidyizdb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hfwhplln.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3fobfnzxh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eeaewyme.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3snpwbnpx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ffytkxfx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ihjleuwi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gwwrjcmp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ixshiofc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kmcecqns.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yhuxntmg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ccuzphny.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3giqdbdcu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3upsoechi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vpcorvxa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ssubjxzc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zkcspkgz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bucrcujc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqcaiezt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fgsqcdvy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fauwhaew.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3alrdrfnk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hfgoowrm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tmbtmhih.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dpkcswwf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3avpsoryf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dywxkubx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cbchnklb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fxprkfct.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qkewisdb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xdljaeaw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nbdolore.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wutbjuro.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vvdklsza.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qdtbdqpd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qbbosrtl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nrwfazrx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ozwxhpwx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zhduymdb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wftrfuzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umbmhyuv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3hjdxfpjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytjfjghs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pbgfgglk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xoewnvrv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cfytyoyr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yfjuupbf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oshgjgwl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3crnsytmk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3iyslcjev.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nvwwyudu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lrrxcxyk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3eytgsvtr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kjogxjlb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ujoqfvcf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mpptaxxv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xvqyvani.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gteffdbw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nzpudlun.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mtjcvlav.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jxaknqja.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tjbfoysv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ampxipal.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bcdtyklt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bgzyguww.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vtbfnpar.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uycpxyqy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wegnreqk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zqbwdswz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtkthfsl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mkqanuzq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3cgexjizx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tuqqxuof.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3urabyppo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imidmbtc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tdrywyok.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xmzezead.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wrhvqcng.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xlwnptpq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qydjmunf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lvnbdisx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pbglxazl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vqgxvvyg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xnycygju.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rukrjilo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zowcyfwe.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3onrufuey.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcynsmv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3whremjxj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3onfyrodz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3lhrbgjxt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hrljmhix.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vnqpowta.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lhtiudpu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kvaijefa.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3etvkqjks.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tnpfclun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbcivyib.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrnhvwkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umgubhqp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pcyebhez.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xbvrhjzh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3acsyluju.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jctaclws.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3otbuzbwl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bqxxihqt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rhawizst.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3afpwviqn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rznqrhbv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nmfmrkcf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3uzowrbkx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pxkwsvfb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zabnhbyz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3oniotvuv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qxnvxzkc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3emfcnwzi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3cptdtjls.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wjqzyhgg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uivcwfyx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fdsbvhwi.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dnccpoou.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3opdttndz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dfzbxvii.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rsidnncf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3grshinsw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kzwdmkhv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3nkxrptak.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3dvupbebd.html


<!-- 参考信息 -->