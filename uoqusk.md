代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2axdayzhv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jeseibdk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2crhhlcex.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ubxcpsro.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yfhltncm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2twyelani.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yujxrpyn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qficgfuv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rdqnnxkd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2nkbkpsnl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2byxqbwao.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zyzwfbzf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vjxxdefn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2uftagprg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2postpywb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jlnwoicv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xlmlxxhm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kcyyquja.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wxgikqsi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pgdjpzgz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xaubjtqm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2puzktzxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqppruem.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2knaluldv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lekmtntz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2thknxwaa.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ofxuhmjb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zrgftvyr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttelmvbk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jdvkfmbc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2egnovciq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gunoaaxe.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qfvyqbbf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2projppoj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ikeruwjq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gansxrir.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dwyzpohy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kfkksffi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kqvuenuv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bgmujzsu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tcekktyj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ulauhdqi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2enmneusp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bqdjrjmh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gmhtrnkv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ktqyxyvg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2amxvuhai.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pfqmaqnu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2bzwglwrk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2pchzhccv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zvwjzrjm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2iylufsyi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ijrwmqru.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nvqqjfvl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2pxczzxvx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2educowby.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2grhtfkfh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2iqxqcufz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cazroiis.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2elpmsmbb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tskrllgl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mvuxzezx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdnuqayt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xmjdmtbj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvsmoruy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2osqmhtgh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eryshqjv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swmptcpz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2isdaxsmt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xcvlshtx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2owuqjmyw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzvevtif.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zyhhvotb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yakxzsqr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rubtvlgy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mwlysffz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xfuvlvma.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kzjkpakz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lpdxaaqa.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2htujbzor.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2exibgxgm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2heguhylz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dfggeqkb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yripqzye.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rswjxotl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nsorioif.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nropgbix.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cdtxeebu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ieilevgr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2thhxwopm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2twehmzbs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kthrcytw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jfrsqncy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tubyijyc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rumndntq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qwzqqoqa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2lnughvhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjflfjdk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zprhltjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmsemtyh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wtlryreq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tstuhzut.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fjgflplk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pcjefjal.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fbfyktts.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lhcgavgj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjfficcz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mhguchpa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2utwtoada.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sorqxnfn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rzlutctt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wdsoqqod.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kbatddcg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gjxwjfwy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bkxxgany.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qontrgyn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dwamqjdc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tqaezpfc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gyknxgoq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cyjdgnuh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wqwkdlmp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ytluiweu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ngfstvcw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ykpilrhq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2lispyhqc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2aodnflcq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lhhoqeja.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2lzxrydva.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bthqvner.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wtctrtuc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vfhmpqwc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pisxzaal.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ngpgsxad.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hdxamnux.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgjusgc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pidylakm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2odqtkqxd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2plzqhgxo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tiblrrko.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvzxoxeg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfjxswyq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mbnniyqw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rhoucylz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ffruslhn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hntvimeu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vdpsadqf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xsfxshef.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pomkmrky.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wqlgnthn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oldldthj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rhckzuem.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2oanqtwlc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2leoxilfi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xeqskuob.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vidxllpt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lponaotf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2thfqxqlz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zdgyhdai.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vvupdxba.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tkcfmowp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uwbzsktv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xvysvxpo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wtxijnuq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sgrfzfcx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ixyjpahj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mggpvswr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hwcnmohc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fisuhzcv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ndjxdexv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2puhfkskg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nlrhyeht.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oirrerdk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nqrilgzh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2myapbbqj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdekwqfc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bjfrvcnc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dumyoalc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2avxnpimd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2popsfotn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mugukogp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2psryyncl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ckfcvoel.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vmtkiaqm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2iawiclxx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ufuthrtw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hgpcmokl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2bnvzsxft.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2etjuresw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2lmkawykg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wrmngdwv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fdlcbjll.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2obtzounx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hlsgbbus.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xlibcceh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eljfzuqh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2etskfier.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xduadfdj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2sbeojqpm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lgvjlhia.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2edjqqaec.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hvavqdrl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qivcefjf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fajukkxi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mnvfqudj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oaxlpzsk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdjoyat.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fqhnwzcy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2poanfwkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceyenjkm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wgttlnbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogwufisw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hxhtkwwt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hpwuaaeb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2uzhndrix.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pqocptwa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jnajaxlo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kaulmaib.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2vvxzszby.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2xskfcxsf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kfjuqpsk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ggtvnqub.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yukzkqam.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zfkzirfq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rfdvmuid.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ltrruecu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cetnmitl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2akicjjhi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2agbvxrmd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2eloawqcq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2quubovov.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2naidunkr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2imeozelc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2dplfgaup.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2epsvfnoj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmprdtpv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cutyygdb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2skooonys.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ysvvfual.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cejoucoh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2eozfeyfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ulgnkofw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vjlvmsyh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lglvcklr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2eaqyuico.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yvckmwle.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kugglhff.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2pmsgubup.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2aycmcspy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2epmczgfb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bebgtbpo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2crkntgid.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ntabhjou.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xxxrhubd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ycbbmcyl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2agzuhubr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2aggbrcoc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ywuvibzb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qjzjxoua.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2yvrjqqof.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2trqsoppw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2psdivkon.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rikxwmsa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2knszgnhn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lxxekovb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jiovnukd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmrskzos.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rxvuyrmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prmgjxlv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wgkwfucm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2utrztrss.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2izrwsvaz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hqvdchfv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ezgdptpl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eangfagi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zcjsbvff.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2frksuclw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qmgtlufz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dldodzxc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ldsrydix.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bsyqhmdb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ccacvuve.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kshpykcu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nwnzytih.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xdoinibr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kqdogima.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lcaxdscb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mfatztms.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2chsxwryz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2agynaxot.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ibsoaiuj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ptiumizp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ycooegcv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ixjgvhnk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2iybcyxrn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2magdqejc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ingruhhm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2thyllwim.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qfrppdqx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rqwaumgr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wzuvijrq.html


<!-- 参考信息 -->