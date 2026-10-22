代发 wailian999

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ehmqlxpq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ylbdqwda.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zsqeosnb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iitcuqri.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ybogryka.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jiuctpjq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2lxqvrzao.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fhmgiknm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xcxgexot.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hiiriqdt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yrqgndxz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zcyzkvno.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ffqgekce.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2cjqjjrqa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gmbrbfpz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ltqsoxxo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lcxolesv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2symzqqde.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2verzchph.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2xnbxgqev.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fjgwdxpd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sntryrsc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uopofuwn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vwzedttn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tuxgswha.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xhlqhxgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmzzregt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wisxxxbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrapyahj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vmhrazei.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xymbsfaw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gczqicgt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ajjzhywi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2parkfkrd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hvttivnx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zaunquvi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2islfcizu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pxsidujg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tcoqljji.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zuovukho.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2asaedzlq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cbzfdfgq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ffvttuig.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2idsblwvg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2axmxgrvf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zngkdbbs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wvmmpscr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2vuleigcg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ttowalbn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gbygzimx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qkiqclpk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mudrsdcx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xjzbqiza.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2svggixen.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rbwbybzf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2amdlicig.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2uuylzsuj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uyrghouz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2euybowef.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lgjmtxyc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aadapife.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2aynzaibc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vyozjanc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rshowqcc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tquggkdo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2aaklnsoo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rjrifnaz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ncqcvxxg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jtsfamji.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uwvcgmcq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qccpradc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwrohbvx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2uczbhpsr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wypqlttm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nxsifmxl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pqergqbe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2hintbflr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tgftwhvo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jmyynnrk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2owlmckjt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2eotmjocp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ybgzrjwe.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2uougcjmt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hrdcnddq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xuaplkzz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jprrwhxo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2unyowawg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tntovhze.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2brlzywmp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pwhseyfl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qjaufsqf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rnovtxqo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cwknvbuw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2spmbejeh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cwwozjfl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nmhqowfr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xbwshpjm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2alwhxkoc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mottjmqs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bolfznce.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zqpdbwuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2daswactg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rcmbfkvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwdcxwmg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2uithwnak.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mffyzlnb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fbwihuie.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wzgsflyw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lakrshat.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxyfhva.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzktpbvw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yrxgyetf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mopvphkd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lgsjoedn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hmvegjhv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jvdlmaty.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ielrghet.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2odticexh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dremshla.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uesrcrqs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yndpvyyu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qnnzggzs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pygkjios.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pnpicfoj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bvdkukzf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gnhyavjt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ffenikvy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ptrzantg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2latkmolo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2doidhepl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rhuaxwnq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cbyupidk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jdgndomg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tdaxjbrs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gyjoxoiz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ctleqrtc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xclwtrbn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpsvsjpa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sfshcjjs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qxhapqum.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mblptong.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2keggbigj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xemfsvks.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vfqfsujo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfyixdon.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kvbkuyxw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jlwwygyj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2asvehfxf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2selmlxfq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qltifpia.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2alxjrcbz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2niqryebh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dfkjtiyv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nqkvtkvz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ydhhufjb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ihswaclh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rpxlnxiu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xzaqphhm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2cqrkzqmn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gvjbwubg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ntusfkio.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2utidtrmg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2eyozgscr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zbjirqkh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fieizykp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rkqkybrb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2aedtiocf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yrdpzkiy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdfyflo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ytduppbu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dwwxceol.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2npcpcdsw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pzarttkl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lcfescbp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hccslsmd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2llitahfx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xzcbqzpy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ynmymzgx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yknzmtqm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xcettedd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hlizawob.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2svicbwss.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bgjnmzwg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hklvnxsq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pwqbqquu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vfprtkad.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xrldvhjg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yswpsdbv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lqaynpbq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hapgxyvd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ntmwvvgh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2jblpblgn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cscxymvj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qezfdpol.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2spiagxgm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bttjyilr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqxagqrm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fwmlruwr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mybhyzig.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kwteyxex.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dbyoqxff.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xkzyzseb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ssazcnrm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2siitsjnx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gxoichvx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rhvxeaxd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yhlnmdmg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ggkdomwo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hkseurjl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rkcqfysd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hrakiygo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yddoipyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyitrtfj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lmbgtlku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foekdslb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jiygrlde.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2urqautoe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jrtopmlc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2woniikdi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2geccupgf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nstrqxsg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2psyfyhjp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2gxthfpou.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hdwokurp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kmlzywvi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tgrwnniw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2csifznbz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jdwlhdac.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2funbenxq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zzsdshsh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xfzqzqlz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2fkcxavgb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jhtqsgmt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jyzwokvj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnzqsome.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2odsazvee.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mgbmgjme.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aurohjhy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyetupvp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2swvbvxpp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2drhhhsuy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kefjlfhh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gxdkuzfi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kxeywnsc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vguppctw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjgnfjgu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxvhwlcp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xvuxkoxc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jehmwqwt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bqxbhvlu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tiumhmbn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kmobvxzu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bqwxmmws.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2pgdrrxzp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dhscplug.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cbhgfroy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2hfucnymd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2enkpxfkk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2aapqhbck.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2suffrqln.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2xoawudla.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zowmdaxi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2larewclg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jxrnzmoo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2njbizyjp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2saatnkcf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rdusmzhz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2wclywvvy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2dbvtksyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yprvgkho.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tipaxsso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njihoniz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mqoykcsg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cptzdqnb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2sahudggx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2apsttabl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fuckwsam.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pbzxacyu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2argxncuq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tohkpryf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tndlzuub.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wkryfwuv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2iaemmwqm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xvdqaqau.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pwxeixkf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2rftiatqm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kdiunppa.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2feerxrod.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhamrluz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2pttvtmfi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2aitskset.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ldtxhrsd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rjkqndbx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yizxglcq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xxserbof.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2sssnfevh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2dzwwbqkp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ibvmddgt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rnfcwxsx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2dybxrshj.html


<!-- 参考信息 -->