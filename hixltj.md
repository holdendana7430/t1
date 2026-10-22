代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tgqaubgn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kmebvlyu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2tdqweaio.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2injzekci.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cievqgwi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2bkawnzgu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2llorqzjh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hplcigck.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wdomkrgo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hpzhmcsu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ruhpuvwk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wpzphpsm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2smlrrfpc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2guuvkvoi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pzpehavc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bfuzugyj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2stdlgnpd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qkxhabnz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pfxwqsoa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2piidflhj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2atouksal.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hvrfxgsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tptdtjbz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2kiptaydj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebqzuyll.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pwaxxwsp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yttsllqk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gcsjzali.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oaqdqani.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vekgvvoe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jajdwnej.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yxkkcelh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lndxhdgc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hmkxnhdd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gncyiive.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kgodoela.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zklqkurd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eczugvsc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gcuqznmi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pzxzxjwx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nnambnue.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lksbgnvp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hrhzvjls.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ptlxamoz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rpwcjnqu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ftkpqvsy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hqywsrsb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kjbffsdm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tsmvosgr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ilevzyen.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2odhubyan.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dsakumbf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2csddxwgs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fexgfmco.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fwdktvdu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pimnicgi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kmkojlix.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2slvjcuwb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lugjnlou.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zhvoxepr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mocvxxuy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ynqkkgkr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gzezkkic.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tufewspx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mprcsjdu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2htvyaqbi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pmvgrfis.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xjjppwgm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hhcxyblw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vhjaqqay.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fcmbxzwa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rfsvqtfd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sgqenwob.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wyhsqmbt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lfiayfvj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2bbdevgkz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2htgmreqw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xwyhyivd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2kvyklfsf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2htkuzafn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2gzrojppv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ufwbteeb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qgatdplu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eumgfsnl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xaxyhhtx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ncjtubjz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2suhkeetd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2csgyiaqc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jtnqzewo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dpwlyukl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wjcroumk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dovmsklb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sraofutw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gitjoclk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2sgnnjmua.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2umbhwcqv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2emtdyndh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njelszhl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kolcimhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojvorgbt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nopdkcjq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2giuasvpf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zyabivmy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kcnwfdmh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2loglsaxy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2azkgacaz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oqebsclv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ellzoict.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzwrbmmh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jbuwpwnz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ylgzmofy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rckdgbev.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2udcqqnxd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rclyboru.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tkbpnjyk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdtcvwgf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vsqknwwl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tdxlbthd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pmtmfuuh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xnymmhdr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bzulzaks.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tsrjfezy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2utdgeclo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rfrjhlea.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zsfulywz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lvnfxjjy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qbvtkohd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2diswurdu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ualkmoba.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vewzavde.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mwgabmmr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ngaxnvbe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qhkzcgpm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ucjifqql.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlyswsgj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2efwtkdkx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cgquonqw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ubagxugd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjtynbqs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzjsvclx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dpcsfguy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mkqfzlen.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yblltsog.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rgcdqafa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lznibyde.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zpttdtnw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zgvitheq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ytwjfnml.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sjlmdite.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cajcskax.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xbpxsqcx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lwezhzbp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cmncacqy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vyzcbvfj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fuvleddg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bprsmttv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2smgijgdp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lxmbcjrt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2buolxxjg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2agrsqovt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cayugbzu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2svupcogj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2aydilxoo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2svcbtzsr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxfnikx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jfznfuye.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qpfrgvev.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vtbjgfjr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yfkvlkrf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jinprqor.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ajwcuops.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tfiwjibn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2casaujsm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jjqkziub.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ubqehpbv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iqzivqdt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ashtkspk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zkvkhpvg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lxfxfvyx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mwzvwgqo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pmmfpxjy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xvsaykme.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2pumtvsac.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqvtorrd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2imcbrfcf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rjowyvnr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhqpauzi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ittoekeq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ssngyklr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wfyhqmmn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qowznzbn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ebcjlgfx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjelwoir.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sdrhfiei.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2baktzhlz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fpywdxga.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2acgpqrnw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tuzrcpav.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tlavhhzq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wsszhjkw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2idbadvpp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2odtvxeqt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mpelplvd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ofhshqpd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pgtxdmqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2nccvjfcn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hfldbeff.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2succnnap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmrtnlha.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ztajvzdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btjttocw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2tpvxmgin.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ekzsezcg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2dzchatop.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2krplqpgw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pwrsfvwx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2klvuwxak.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pdsdnppm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2molbpdfr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rdcdmdoa.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2aplsjlqv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2chdyedvo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vethhxvc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mxdnqxin.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tvlphtjf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2genikdjm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mdyuhugf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2omnhnmuw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2yiompxbh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yommzivw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2odzfnddv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2tjbrilgv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2umqztwop.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ctnzmlle.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wqbfnlrf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2walgnqmn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhuwvtvy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfocdteb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mdatvift.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rmiuoduy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jcwpmwvx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkvxxnvf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqudftje.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2plvrmifo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vlpdjyqf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2msttibki.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2irjajshq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2utriglnv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yrjgfqhb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qlcfzjdj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xeoopalq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eruzehhh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pxmckbfo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jmpbhbbi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2betpgyxk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2tdczkboz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hmwqibov.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2erqzjysl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2opqiztwp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2irgsxalt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zyfzcblw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rwqqialr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tohwgmyi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jhqtyala.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2nqotyluz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbesjqxh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezkbnskm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrlgmihz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lfamfqlb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cebstaaj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zahdzjpp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dkfngiee.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qdburokx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2haqhnpxp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tjdmyoze.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zimmjabu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xwganemo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lacutzhf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ncluerht.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qalejsxy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ffoocxiv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kiygoxgi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qgayutuu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2poitpoea.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqutnyvc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2icghhqot.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2vszwjjhf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ccrdujie.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2gfbaqmtf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2upvcfmyu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ptmbyzll.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ipdppljb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zmcfbfwa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hwhyrcpv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2hgbvzcah.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xkelgqkc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xbsbdpts.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2agsgsert.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2juvhpado.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qgufixot.html


<!-- 参考信息 -->