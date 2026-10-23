代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jwapyrtl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lvcjdtsu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3maficijs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hqjbfghc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3mmeicjvx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hlcxlwzd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3djylldzr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3otozqgut.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wijivoda.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3avmedtfu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ahviylxm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3rnnzluwc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rmbquiad.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3bwbpgrih.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hnlignfz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pkkldgql.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ybidtrpc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3psfxmzkg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qoeiezdh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ptniewaz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nnvuhxwg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lucdykfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grktlumf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yjekqwjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epahpwar.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3skailvku.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3adzwoefa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fjalcjll.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3maszrefg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cdwsdemc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3eqcoqwaj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ywqinrzy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qfrgowre.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pdnqzfiu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rkarxjcj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3juduvfyg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ikvmpvpa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3eaxluuki.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pteawoop.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3szwahcqr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ayxxuwml.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tbtxattw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mlzbodtt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kldfbbyt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qkcwrvjp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3okhrllfn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ftqqwnha.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3muttjrgz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yzmgqfou.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3neikkmui.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3eczqxgfz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lmmikvvc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tgpmlpqf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3nfnasfeo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vyjvymap.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pqfvqpej.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3epwphbyb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vtgkmjfd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3chchwpjt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3nnrqscqq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ccikylue.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ixhnqdtv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3loglhocy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iikipnlh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dxgqdepj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3emcmkwiv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rjlqavqq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gfmzwzms.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3iokltsug.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3srxerrqm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xnqvgrrl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nujamjei.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yjicdlcq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eopfgfbm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3janohkpr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3biqnnhdk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqromfs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nploxkhi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mqxtffvf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cbxbfvwl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3yazhmpsm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3nmnzvqom.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3krhpzmot.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rvyvlqsc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nbfqekgl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zewrwofc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tbsdzgxc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3evrlvxby.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3scauqfad.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qoyjkuvd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bayitcmh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kylmmygv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3esknpicd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zouzlqet.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bznaydfy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3lbevoxbs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ukgocheq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fchcjcso.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3nlwcfctq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vytmrjfa.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ydddaznk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3twkqyzei.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jpssxurr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wfuwdchb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rxlxjlvl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrbnqpoi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3efevrpis.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wfaqlkqz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dacfuesq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gsawqutu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cpxvzdvb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3omhpcona.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yvurlgca.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vjblimrl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ocnbafjm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vjghjvgr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ybmtskwh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nswkkczu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jybakyvi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zygkpzbf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nyutugim.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fsruuyts.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ayhabqwx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qtsoqdna.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bhlzcoqx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wgdnhzwk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lngrvkmh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dbjxnitq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lxfolcnz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vclvwsqi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qeequlin.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkxnfuwm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifmowezp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zxvsonud.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wufpdhid.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3okcxbcrc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3koymomoe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3itqkjlpt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3cgaltscz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rxypvepn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ltvyzodg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3izsazfis.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bnwbksgo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3iqtorplw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3leubzmph.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ugosbova.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ktcgbttu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fddcmklx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fafnytlo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ptlvkkig.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hpwszwjq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xquiszde.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zykziyeh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ndoxxymy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ytdveokf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ngsfjbhx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3oqrdobiq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mxtajfxq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3viomhiqp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fmqhupqq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3janqcbje.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hxavpssk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gappssoe.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rkzvfmhr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bapawwnv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cruidwww.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aeutbtoz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nyvocnuw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ghgxjzry.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pzbajtlz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wunfabhz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lcwkzprc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tqodksou.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gpvyugwz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ewhhuwjx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3enrlsdmm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mqqpcyyr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3sdrgnrtn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3twnrutzq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wwidajex.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pxqhvjrb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ovtqyhpf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zeffwyoa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ozvxtpzb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ynecexoh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cpyjcrix.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xhqlqtki.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3orfywyxj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yveosytz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bjdfaayj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zokffrdq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kuoopzge.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tbomkcyx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dcfxvvfn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3czxlqmmd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yaxhnhrv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gcsqgdlp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3enxinlsw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hbpphtxg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3pivdbtyc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tipujomj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3eeivyavl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zszccjfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cwisswlb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jfeeqsql.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tjiagmxt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3mwccurty.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oaqkczwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljuzrxua.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jimqibik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fruccqnl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bzmukumi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vubllfwx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cpdafbwy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3yfyqojnq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bxseiart.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3brlirolv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3shtehkdq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3smafsoht.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ertvhvga.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nxrtcgds.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tuoqsbpt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hwykusyn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3flejghsq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wtnkuzbn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dnoknmda.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zefbemiq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3jimbebhm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vjccvdjm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3efsxbhzz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gxvepuar.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3sxktjuit.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3knxrjyxj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ujoourya.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ozqzfbzg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3taohdawg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3vsmcoemc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ddaxnhbe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cddjcdxd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3skxemkbd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dlxsjzvt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkdctexo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzeeyjuy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jzsylnnl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lrkqswnd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vgniduhn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3edncjxti.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3tqwxgarf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qcqddsdm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vhrbantg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aajfuxtg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qwheufin.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3vuryhdbx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3isicsxwr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3maseiswg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmucuwwo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yaysuhbb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fsfciubo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3lakjnijp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rcomjncc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eyfrzucz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zvporjrs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3biykowsc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3flyekmvw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gnufngsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgtotlky.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3tcdxyvbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mshhuybs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ztpnlnde.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ehaaiheh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sgqknksd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xuhiaryv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pcumgbkt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mibiemma.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dnwwqpvx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3elhvuafm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ecdogyox.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ljxoildo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hqxpbbxp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3daiaeovl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3goptkcpe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3umckvmtj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3valfqfzz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mhrfybou.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrpqbur.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fukyvdma.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3fnqumwka.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fzrmjgtq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3cjpqyodx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkngfww.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ocjerdlj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vkagjlas.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ztwryebv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vwbcegai.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3kidbasyc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3yhyfxmjr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3nmzwxgwe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lxefxsge.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3iexyycfb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3riinhuji.html


<!-- 参考信息 -->