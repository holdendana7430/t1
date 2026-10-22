代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fazhgjep.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bhrtlxkb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lgcdleim.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dfwimtnc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pssgqdap.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zmsoamfq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xkoonlld.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qtteyfvu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2usqctswv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2aeojaqdr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uhuezlmu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hxxeugkp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fwcowdfx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tlkqmpgz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rkcvvtpm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2evndvrzc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2brsbucud.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qatdrisn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rdepujrd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2brezuagm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iycqvyjh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sfgydbdk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2vfsposcb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dlvciyra.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vdmkgyum.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2uqevnqzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kouxntyx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2skuxqydy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wutmeuud.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xuqqtfiz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jaasirbv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fwwdcpal.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2erimohul.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ecpaxtyp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vnzddfkz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rdneppwh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2susppgeh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2iocxvxkr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2brspgvcy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ovbpcoip.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aoowvpda.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rxisvmsu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2naulrhod.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dagfuqzi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2enwucmzy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2icxaymyx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2duyrtite.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yqndrdce.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2amqcwvex.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bhwfndom.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2svzzeacj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jyviaojq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lnjawgju.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hrrahyux.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zlvvupjj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ukquhhla.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2aaekydrs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bipefmxf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2cjpvlmtm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kisrzgdz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xioxxklv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pskeifti.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nvpriwkv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2icuvfddc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2nnqhbtqp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qgbkgszs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwxvmnze.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2euighosz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lhsbjtmf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wsnopxnz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhonlkjn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzssaaee.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2przsfrxd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2eywjzmri.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zgutembp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzuaxhq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jvhmyhrj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sxfohnhv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fvlhpktn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dmknvgvi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vgsbxpyz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xulhnfzr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zqrwrvgo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mklfiluq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gtzdhyjj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mwhlrqmz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2pahvevum.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ipfkizll.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2joayviku.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2amrgbzyz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2efmphmtu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ufejplty.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lppfzxbu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yneurlvu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2itcpenca.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2edjrlnnf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2plvnceas.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lkdscjcf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2umbffgga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bgatymla.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2akkhwfyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcqrcfuw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nlnlbllm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbvflgov.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mcsohery.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2apouwjwy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qowhvvgb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cgrvnyfb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2phpzqifr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcgpmtli.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bycpzccz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2byutyymh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yzqabpzc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lkvgikxs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ibzhllrr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2swyqdwov.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwoarvjo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ocknakou.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wpuoxrkw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pinxrfzw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uzuumwlo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bcbjctfu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fuzvurgz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mhbplgez.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ksfwhulk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2cpwswvou.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2abwihpjd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ydwolizm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jlabkniz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rtmtchec.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2beupmxwd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gxogkqhp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ficzyiks.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uueihblf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vpiiaiez.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mrtgwijd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdtktrs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2asjrazni.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ahruvphs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jkhffmfa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nmdfiwbb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpfsyxc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jegeyese.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aadcgzlj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jgnuomzf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wgxzetxz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2mrtdvmfa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iqfasstz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lysqjgmo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2gxxnwylo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2njkfixdv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2batncfml.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hautgfbp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kosxekul.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ingkcrhh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xlxavtqv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ugevuqvt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oablerrs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vajssavt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tkdnynsq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nbhttxll.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hfhcawte.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vonmmbfm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vokxmgqu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tvspikkm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zfvkyuqd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gzyphoyp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2broqkejj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbhbdhly.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mbeotkmj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nhxodwdn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2plkfinwx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ascphkaq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uikmrutm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bnunboti.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wbfzqskj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dxmkgtcw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2otqzfgws.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mhdwtvuu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zqjbkqca.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dygtwuoh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kdpmoxin.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vvlbihnv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2virblalh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bgijomeg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2eeoypgyw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2snchumem.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmdyuuoj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2gyspeuxn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tagnyvcl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xdmkdzgp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwjudwb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2swisohdy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlupnzwm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nadvpyze.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2pyrfkseg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ckfwxuze.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qemdoqek.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ypyakzrw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wpevquwl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eptpljhc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2srlueobv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qiedazdf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2wyeexwdd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2thlisdxm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2etnboijh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hpijmmlx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ofkfzwjm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2owgoyrry.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xfdceuoo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2xrdrwwsv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ntijcfyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wiuhxzpj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2osztbppg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fttoesjm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bmkfsxva.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qyhnizaj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lwxmaiuh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cuiizfey.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2grhbxloh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uglfbfym.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2umgzqtnp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2aaalgxfh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ffpljdxw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2emlsumkd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2oynjxgbr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2opipeauh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lwaiwxpc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ctciymoe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kprhdmnz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2nqeedbdj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2eiqpugdo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wajuhdnf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nvrzgqva.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vuwesobq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2uqjjrhus.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qhewulii.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bdospgwm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmxsiodc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2uqkitgge.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sfrbljye.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2husojekv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2lgoptkwz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wqtwgjec.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2epszfpdp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dexuoxwv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jnsebpzf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xulkeajw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ulpmnyiu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2payonncx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2glvwfnih.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zhcapgui.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2opkuxssv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2clumlijd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yuokwfek.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2byapbwcd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ilpajdkn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ilxlnxwn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwwsrrq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdkkmhu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2nicslqdi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wrrczlxa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2tlwocxnh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2duutbkej.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qjlxccbh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bihyewcd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cutdmprb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gjhzlapf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zkbstaue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujppjeyh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2wdypdncm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhezutlc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zwukrkwp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nnftezrv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ausnfozf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eigqgfpk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xvdpvtfy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gacmbrfe.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2awcqvojp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xusigrhc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wdgwzrwz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mkjirjli.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pvdhvwfd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2izwrnrcu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bvhuaoel.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zijoizwm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vhilpjmh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tjsahhvl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbawykb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zjvwsuwh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbgevkve.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2bohskjut.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2nfgvalle.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qeexevrm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ytputexz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2fygtwtqg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cynazuvm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mbsimnpe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ajcvwapg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bhgemcee.html


<!-- 参考信息 -->