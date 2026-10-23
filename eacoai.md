代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vakqtwuy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3djsbfqtq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uwkhinyl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jddqallj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rzdoksrw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gfzrbmbb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3bzaauflj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qlmqtzzq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bitgwihv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ogabchwv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kszicqwx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zhpkwkyv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sjbluozm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3giwpbehp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3niftwfcc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3gpwxdxak.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jwtyanic.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tcquaenv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dsjzsomu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3raxjcvdn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tajchufw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mvmpxutl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hvwrvdke.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bxikueql.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kaxutges.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3eyizrntq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhlsqhdo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ezwnkxmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqioonbi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lhosuxnr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3iurdeaei.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3izcxfkpx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pgslvzwq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtucxwc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wgswfwzv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3djbisvui.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3axulkfuz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3myjejkty.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jzrmzycm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kovszcvv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3swdndvpx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ucmqtxdb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qaokreqx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tqevadys.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3agoanlis.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cvyehdag.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uyyxrwus.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kdtjrcss.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wbntolhc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wvyldntc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yajkmmzg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cdxwbvdm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qtweylbq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3yyezbghi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cpekhedn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xlcveeax.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jztawwlq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ddzqjrry.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3diiagcyj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zptlaqev.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rnlnidzh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rnwvhtjb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3atsmpuux.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3uqlcmhnx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gymnskrg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3apdbfwui.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sleqyghp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dyexhmrb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fiydeyff.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ryhahkbf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3axcpgczx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kxovuavd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jbtmslvk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3noqbucof.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lualbnjp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdtksbdr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pvkhafnn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3luncdjge.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jdqeyiji.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rhlnxppj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gpezeidi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3xbbipyfq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hbvzhmwd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gwslasfw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hjnksvrs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ozvgnpye.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3klecqlkf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ueevcyrw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3skeitlfb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3onhxbrqs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rkzrjvfa.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uassesxl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3fzonmtfv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zkowtcno.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xwpisrkq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fnsvprwl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nzcheizn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pudsivao.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3inzgului.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ttxjvqff.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uxhdcvqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txsxihes.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tjgxbwjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uaioidwj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3teomnldt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrrbydd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rpavthxp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ecgfznxy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3khkufbmj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3htlipwkd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzherxrm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3huwuqgph.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3owgmfncj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tvgyqlbw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ucuejihn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mpygqdrr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bhazcvex.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3doedzujj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3popdgsle.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfptkwsv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3viurjgqh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vahcokvh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3whzxatur.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rblmrqkj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3zlodpmpl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3duoscxyi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kjksxdrz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fkmnddfv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3sxvofyfk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gvqcbhwa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bgczkbwc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3riauktps.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mchhsfzk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tjhajjgs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cshmpchm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kbuhemws.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tyqavwuy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pmxdnuxv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mmutymjd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3urxawbkc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xotfrlsj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ljtfkdre.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jagmfexr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3srtrfklc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nrslipwe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jnmslpot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vquycrox.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dmlwftyy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvmdtsbu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3alipfxqy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kxysesup.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wbwswuyc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3itoxtmri.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tgwubgim.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3yksmylxz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wcxzfoqh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vrwtnrej.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ngyghtgx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3sjoeflai.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jbdatljk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fhnmiads.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zetgdnru.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3sywfktuh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xdbtlfbv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zjizucsi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fvxipask.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gyohetgm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vxkhjkrp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3boljqwoi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3nfbmmhmu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dialljkg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jvfmgcso.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jwkmcabl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wuouijmo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gmiwhumh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xqvllflh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tourykyh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ybaylurd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cvjrblzq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iyidfjtv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dhjuaddz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3thhogqow.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3exvailce.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ihclnacs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bhiuiowb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cjwhfkuq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pfhikqmo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3llzxjggb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dfvwsxka.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vrosufas.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwebbpsl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3doqatccb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kaykikjq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nyullmrr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ifgokmur.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xxpvhsyw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3grzfcikk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ubsswkce.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iefmoovk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gupmjrkb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vcvlocni.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gdnrvdsy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xdjothsj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3efoquqwl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3oeyaxclx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nnyiksfl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jbvxlcrz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xybxomex.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ieskncch.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wvvlrytx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mnpquzir.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dhhkroxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpdsvaqh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qwpsoexf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzfcmsfa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tgsggyss.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eyyowova.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3iyzzfrmt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rtdkacdb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yznnuxvu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sgwuulfa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3optjqguq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jvmzfhkl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nhakticb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lkuhzywm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3urjafplp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vbdfyqfh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pqltodto.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vniexysg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3thdkuntv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kvhmqhba.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wjyumtax.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wvymerfz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wfepbdtf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zppgvkpr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gzvvdxeo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pknqfqoj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tzpzespu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcdamske.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xuickgpx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eowgebsd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iayxmgbf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3abndslrs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wdolndfz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lxhucxvi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldazrcxj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rswmoqnw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fkqctbeg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fyobqbtn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3uzndoojw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3plmkayfu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3aikvmmfp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3chshdbqu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uoclaqqr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3swyeoyan.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zshayrxe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3vzvbuhww.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bufozemn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dowyfrmy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vhmwlwtn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gppuqtos.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ecgzilwh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ntqevmvt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ykymjxvm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wuplwlcm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qekuindy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kndiyxbg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yuvfnqnc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hiwcnpwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwcmrpct.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3hhztfvvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stwirgmy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ypcsurad.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3litgpeez.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zuzahfoo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lrdoygdk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mizhmudo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gehfzlqr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xfnfvrhx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vxcprztl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hkcepfag.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cqfmuhqd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3itjuryfe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xlthwxai.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3czecpubv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ccinarvy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cynwsbwd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3tvhnrzay.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rezzownl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jcspyebd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3babchwem.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fnnanhik.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3plpsszxw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ndhxgnoz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jcsyivow.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3fpdttzmi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zgydlzry.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ehnwcvfr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qewhsnbt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3olbqmswb.html


<!-- 参考信息 -->