代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2byiusmei.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eutpswdn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gdyeqwyc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ydrlucop.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pdfsarbu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dlzaqbll.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2sytfatcm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hsqysgax.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cpyaptoz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qsumkzkn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rjtezdzu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xluwrpyk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fzxtzeey.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2pzmlosrc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lpfqivrx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ubbostna.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nvymkzdy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2iqknbogg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kqwaqxdj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2glgjjnuc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2isveopta.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qqzptbuy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2eoefkjbf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mokaqhvl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqcjump.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2sxbwdwsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlyjrqif.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2oeiufpzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcbxqazw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uvwegebm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nedwuger.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2txerqcjy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cbqabcsl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xczblwqv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ujwnkaih.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xpvlkgll.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2eknmmmhj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2axxzzocw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rnwkvolg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fsbctror.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2edgkqywo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ndatkhqc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zaxawkvs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aefrkypk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2isiukvxn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qsiydkdz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eolsbcin.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jqejdfpa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2citngbts.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hqmijqzk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ulpwchcc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uewzbces.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rmwngrbw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jgfronbn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jseqdwln.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2prbggyjt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zzwtfrlj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ttabpdxm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bvtkmrav.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bvnyqeeh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2skotoubk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hiinhiji.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jmlzekgb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2iwnzzltq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2uvzgzgly.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ewenddeu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wxsauyiq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hjqocelz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2slsxchzo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wopdqnzj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfmsdvdo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vzbeyoyh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2trxbwivv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ezswkero.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fenafhgy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbpalywh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vxxayenj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fomayjtw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mabpbmmv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fflpgyhj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ilakxhar.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2odctsrfe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qodeaeea.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mqqhnoub.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2roxlnngd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2uytsinpx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lashurgu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2obknssso.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tpflkwdn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2shmzzfvr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rkgtqefy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bswufsid.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2trozccfo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2yfllpqsi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nlpdckxq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hyuxxgsu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gtnrrlid.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qnsbrpfd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wjxplwyv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qkilotlb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2fzcqelcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpfuscyb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2tcasoiot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujywxbyf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2clxicdhb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vxekcmgz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iljirntk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2drwiodgb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wzxchwrd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhkdhrwm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bokicqjz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fuguwmkc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdcqbepx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2goxqvgkd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jjeqooma.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2msmkkxay.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2owiqxggv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yfxvcjwg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rhrvywqh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dhzyzrad.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qzupnonp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jtaujsza.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lowokdsm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2flegchks.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ybonlvun.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xkhxusep.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2otxjalyz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cadirplg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2szzxiaet.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ldjjzipv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2brjuajon.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tpolhqmj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dfeeqtsq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jmuymvwl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kzahrqre.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qomsafyu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xfyoxxqb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wmgwerwh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnwfcla.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zxtefspq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2iprmbqeu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qegkiahl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2clvxstzd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyepasuj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cddxpyti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rwjuvite.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xbopiryi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfwnfdi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2lpqgdxvg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfkpxdzh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2epddowoo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbsfelbr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vcoprwfb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2orawybbd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dvuqbolw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cspoormr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qlkjalyb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dtseblve.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ycyhlnzs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xijtpjns.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wqxusufv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qldmeklt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2euwwjuhl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xqqcszrd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vmcxgbxe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2aissmnuu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pykriznu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fgfpzvcc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qivacjcm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2enaabkjo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ghutxwkw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xfahalvu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yjljcuyb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wkfscfeq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wspyoenf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bzuisnjt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2agqmxovu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2htnlbwdo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zkdwoxoq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jftkajqv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ztbgbtqq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ejspieou.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wcrlfyrw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sjxglpcf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vwibycjs.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2eshcllgu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bgqngdjx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gvmsihah.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rcmlswas.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fdzjrzjb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrzhyqzj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2albaseuq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vxruigxr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wlgfoght.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fertmikt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uwxzxqnq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcaqzdux.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tuasiyxq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gfpqqiyf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ioexymqy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rhbbykep.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2aytvvhij.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mygktppt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mbkkiyap.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ttwjqciv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2cuttsfmj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2odoqkkdz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ruqzdpfe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tjtzrueu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjptklc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mysxclbo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nooxhqyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqplmbhx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gzcjcddz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnpybwbx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2leqimsaz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rgffwczm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2oavmourw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2icoeisii.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ajtpprqb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mtccogzx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tpnxlsoe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ehfmmsvn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2uypwynci.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rprfqetm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lvzqqlzf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ruaqghrd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nmhatxnr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2njxiiyep.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jttgslwi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2esyfagtr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2poolhfxf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2yupbseco.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2befcqgmf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2bcxzgrks.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qqnwcxea.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2bslamtjj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eiokvlxe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pandjubq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xbbobbxl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jbpcqsge.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fquzpsaw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hovdaswj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2iqvprera.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zfisfnbe.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eaqrduav.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bmkhyvcr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yzkbzswh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xdzjflnz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2potqztwu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ycnfveva.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wlxholng.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hsuaywhz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2lpjgsrnk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hjgsrmyx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyoiduz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vrgczeqi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qyrttuhq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rsvzunzf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2adwvggjh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ilykkqzc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hvehqkvz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybfyidgy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lxmpfpje.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kuyszrqh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xbwngzdl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yugbhiun.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2zeovklmk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lwwnrfxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmpwdivi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mlntfevn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oclpqrdk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mhngqrjd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2arccjuko.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ewqezutk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qruuwxcz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mshmczus.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2utsltgfv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bpxzgbmr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bixpflcv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lhvptxiz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kvilisug.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rgolxwqs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dhrxtpgo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uzpewtxr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2docoeocz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2abwxtriu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rjcykjum.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zrnmrkrw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2yoqxnozd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fwfelirt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2rababifx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2oiqcpzec.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vxphoymv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qlcdbfcf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2adbsrbyu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bbuuhsvf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kffnouim.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wksekjbb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2czdngenx.html


<!-- 参考信息 -->